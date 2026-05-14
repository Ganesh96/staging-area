```
{
  "system_name": "Rob",
  "task": "Software Engineer 3 (L5) Interview Training",
  "goal": "Master complex distributed systems concepts, architectural trade-offs, and large-scale problem-solving for top-tier tech companies.",
  "learning_topics": [
    {
      "name": "System Design & Microservices",
      "priority": 1,
      "concepts": [
        "Distributed Systems and the CAP Theorem",
        "Microservices Communication: gRPC vs. REST",
        "Service Discovery (e.g., Consul, etcd, Zookeeper)",
        "API Gateways and Distributed Tracing (e.g., OpenTelemetry, Jaeger)"
      ],
      "practice": {
        "coding": "Build a simple gRPC server and client in Python to communicate between two services using Protocol Buffers.",
        "challenge": "Design a globally distributed API Gateway. Discuss request routing, authentication, and rate limiting at scale. How do you handle distributed tracing across services?"
      }
    },
    {
      "name": "Cloud Deployment & Scaling",
      "priority": 1,
      "concepts": [
        "Kubernetes (K8s) Architecture and Core Components",
        "Infrastructure as Code (IaC) with Terraform/CloudFormation",
        "Service Meshes (e.g., Istio, Linkerd)",
        "Observability Stack (Metrics, Logs, Traces) with Prometheus and Grafana"
      ],
      "practice": {
        "coding": "Write a `docker-compose.yml` file to orchestrate a multi-container application (e.g., web app, database, Redis cache).",
        "challenge": "Design an autoscaling strategy for a stateful microservice that processes time-sensitive data. Discuss Horizontal Pod Autoscalers (HPA) and Cluster Autoscaling."
      }
    },
    {
      "name": "Databases & Optimization",
      "priority": 1,
      "concepts": [
        "Distributed Transactions and Consistency Models (strong, eventual)",
        "Database Replication (multi-master, leader/follower) and Consensus Algorithms (Raft, Paxos)",
        "Sharding and Partitioning Strategies for High Cardinality Data",
        "Distributed Caching and Cache Invalidation Strategies"
      ],
      "practice": {
        "coding": "Write a Python script that uses a distributed lock (e.g., with Redis) to ensure concurrent access to a shared resource is safe.",
        "challenge": "Given a global social media user database, design a multi-region replication strategy. Discuss how you'd handle data consistency across regions and resolve read/write conflicts."
      }
    },
    {
      "name": "Event-Driven Architecture",
      "priority": 1,
      "concepts": [
        "Kafka Internals (partitions, consumer groups, offsets)",
        "Stream Processing (e.g., Apache Flink, Spark Streaming)",
        "Idempotent Consumers and Exactly-Once Semantics",
        "Dead-Letter Queues and Message Retries"
      ],
      "practice": {
        "coding": "Implement a Python Kafka producer and a consumer that manages its own offset for fault tolerance.",
        "challenge": "Design a fault-tolerant, exactly-once message processing pipeline for financial transactions. Discuss how you'd handle failures at each stage and ensure data integrity."
      }
    },
    {
      "name": "Performance & Reliability",
      "priority": 2,
      "concepts": [
        "Systematic Performance Profiling (CPU, Memory, I/O)",
        "Chaos Engineering and Fault Injection",
        "Site Reliability Engineering (SRE) Principles",
        "Service Level Objectives (SLOs) and Error Budgets"
      ],
      "practice": {
        "coding": "Write a Python function that uses a circuit breaker pattern with a library like `tenacity` or `pybreaker` for a remote API call.",
        "challenge": "You are tasked with reducing the 99th percentile latency of a critical API from 500ms to 100ms. Outline your systematic approach to identify, diagnose, and mitigate the bottleneck."
      }
    },
    {
      "name": "Design Patterns",
      "priority": 2,
      "concepts": [
        "Circuit Breaker Pattern",
        "Saga Pattern for Distributed Transactions",
        "Leader Election Algorithms",
        "CQRS (Command Query Responsibility Segregation)"
      ],
      "practice": {
        "coding": "Implement the Observer pattern using a message queue for asynchronous, decoupled communication.",
        "challenge": "You need to ensure only one instance of a crucial background job runs at a time across a distributed cluster. Which design pattern or algorithm would you use and how would you implement it?"
      }
    },
    {
      "name": "Frontend ReactJS",
      "priority": 3,
      "concepts": [
        "Advanced State Management (Redux Toolkit, Zustand, Jotai)",
        "Performance Profiling with React DevTools",
        "Server-Side Rendering (SSR) vs. Client-Side Rendering (CSR) vs. SSG",
        "Core Web Vitals and SEO Implications"
      ],
      "practice": {
        "coding": "Create a React component that fetches data using `react-query` and discusses its caching and stale-while-revalidate strategy.",
        "challenge": "Explain the performance implications of SSR vs. CSR for an e-commerce website. When would you choose one over the other, and what are the trade-offs in terms of development complexity?"
      }
    }
  ],
  "mock_interview_prompts": {
    "system_design": [
      "Design a real-time, fault-tolerant analytics pipeline for an e-commerce platform. Discuss how you'd handle schema evolution and high-velocity data.",
      "Design a multi-player online game matchmaking service. Discuss consistency, leader election, and handling of millions of concurrent connections."
    ],
    "live_coding": [
      "Given a list of words, write a Python function to find all anagrams, but also discuss how you would optimize this for a dataset of 100 million words, considering memory and CPU constraints.",
      "Implement a thread-safe cache with a time-to-live (TTL) in Python. Discuss the concurrency primitives you would use and why."
    ],
    "behavioral_questions": [
      "Tell me about a time you made a critical technical mistake. How did you diagnose and fix it, and what did you learn?",
      "Describe the most complex system you have worked on. What was your specific contribution, and what was the biggest technical challenge you had to solve?",
      "Describe a project where you had to make a significant architectural trade-off between performance and consistency. What was your rationale?"
    ]
  },
  "resume_stories": [
    {
      "project": "BestRx Prescription Safety System",
      "story": "I engineered a fault-tolerant API client using a circuit breaker and retry with exponential backoff to handle external service failures, ensuring system reliability under load and preventing 150+ patient safety incidents per month."
    },
    {
      "project": "Maxil Job Recommendation Engine",
      "story": "I designed a scalable recommendation engine using a distributed ETL pipeline with PostgreSQL's `pgvector` extension, and through rigorous tuning of the `IVFFlat` index, achieved sub-50ms latency for millions of vector lookups."
    }
  ]
}
```