# The System Design Primer - Scalability Concepts

#tags: #system-design #scalability #architecture #interview-prep

This primer is a foundational document for understanding scalability, the most critical non-functional requirement in modern system design. It expands on concepts mentioned in the [[Amazon SDE Interview Preparation Guide]].

### 1. Understanding Scalability

Scalability is a system's ability to handle a growing amount of work by adding resources.

- **Vertical Scaling (Scaling Up)**: Increasing the resources of a single server (e.g., more CPU, RAM).
    
    - **Pros**: Simple, no code changes.
        
    - **Cons**: Single point of failure, hardware limit, expensive.
        
- **Horizontal Scaling (Scaling Out)**: Adding more servers to your pool of resources.
    
    - **Pros**: Highly resilient, nearly infinite scale.
        
    - **Cons**: More complex, requires load balancing.
        

**Rule of Thumb**: Always design for horizontal scaling.

### 2. Core Components for Horizontal Scaling

#### A. Load Balancer

A load balancer distributes incoming network traffic across multiple servers.

- **Purpose**: Prevent any single server from becoming a bottleneck and improve availability.
    
- **Algorithms**:
    
    - **Round Robin**: Distributes requests sequentially.
        
    - **Least Connections**: Sends traffic to the server with the fewest active connections.
        
    - **IP Hash**: Ensures a user is consistently sent to the same server.
        
- **Key Insight**: Load balancers introduce redundancy. If one application server fails, the load balancer redirects traffic to healthy servers.
    

#### B. Database Scaling

Databases are often the biggest bottleneck.

- **Replication (Read Scaling)**:
    
    - Create copies (replicas) of the main database.
        
    - A **Primary** database handles all writes (`INSERT`, `UPDATE`, `DELETE`).
        
    - **Replica** databases handle all reads (`SELECT`).
        
    - **Benefit**: Drastically increases the number of concurrent reads the system can handle.
        
- **Sharding / Partitioning (Write Scaling)**:
    
    - Splitting a large database into smaller, more manageable pieces called shards.
        
    - **Sharding Key**: A piece of data (e.g., `userID`, `zip_code`) determines which shard the data lives on.
        
    - **Benefit**: Distributes write operations across multiple servers, allowing for massive write throughput.
        
    - **Tradeoff**: Increased query complexity (might need to query multiple shards).
        

#### C. Caching

A cache is a high-speed data storage layer that stores a subset of transient data, typically so that future requests for that data are served up faster.

- **Core Tool**: [[Redis]], Memcached
    
- **Purpose**: Reduce latency for frequently accessed data and decrease load on your database.
    
- **Common Strategy: Cache-Aside**
    
    1. Application checks the cache for data.
        
    2. **Cache Hit**: Data is in the cache. Return it to the client.
        
    3. **Cache Miss**: Data is not in the cache. a. Query the database. b. Store the result in the cache. c. Return it to the client.
        
- **Key Insight**: Caching embodies the time-space tradeoff; you use more memory to get faster response times.
    

#### D. Asynchronous Processing

Decouple long-running tasks from the main request-response flow.

- **Core Tools**:
    
    - **Message Queues**: [[Apache Kafka]], RabbitMQ, AWS SQS.
        
    - **Task Queues**: [[Celery]].
        
- **Example Workflow**: User uploads a video.
    
    1. The API endpoint immediately returns a `202 Accepted` response.
        
    2. A "video processing" message is placed onto a Kafka topic.
        
    3. A separate fleet of worker services consumes messages from the topic, performs the slow transcoding task, and updates the database upon completion.
        
- **Benefit**: Improves user experience (no waiting) and makes the system more resilient to failures in background tasks.