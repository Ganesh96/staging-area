System: URL Shortener – Requirements & Assumptions

1) Functional Requirements (in scope)
- Accept a long URL and return a short URL.
- Redirect short URL → long URL via HTTP redirect.
- Basic click tracking per short URL (total click count).
- Optional expiry for links (expiration date or TTL).
- Optional custom alias when creating a short URL (if available).
- Simple API + minimal UI (web form) to create short URLs.

2) Out of Scope (for this design)
- User authentication, teams, permissions.
- Advanced analytics (geo, device, referrer breakdown).
- Bulk URL import/export.
- A/B testing, link rotation.
- Mobile apps.

3) Non-functional Requirements
- Read QPS (redirects): target 100k requests/second globally.
- Write QPS (shorten operations): target 1k requests/second.
- Redirect latency: 
  - p95 < 50 ms from edge (excluding network RTT from user to CDN).
- Availability:
  - Redirect path: >= 99.99%
  - URL creation path: >= 99.9%

4) Scale Assumptions
- Total URLs stored: ~1 billion (1e9).
- Daily active users: ~10 million unique users.
- Read:write ratio: ~100:1 (reads much heavier than writes).
- Data retention: URLs and click counters kept “forever” for now (no automatic deletion except manual/expiry).

5) Explicit Priorities / Trade-offs
Rank: 
6) Correctness (no wrong redirects, no lost mappings)
7) Availability (service is up for reads)
8) Latency (fast redirects)

If there is a conflict:
- I will optimize for **correctness over availability** (better to fail closed than send a user to the wrong site).
- I will optimize for **availability over latency** (slightly slower redirect is acceptable if it keeps the system simpler and more reliable).
