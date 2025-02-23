# How We Pay Only $27 for Flexiyo

Flexiyo operates efficiently with a cost-effective infrastructure powered by Railway, Cloudflare, and Wasabi. Here's how our setup is structured:

## Railway Pro Plan

| **Service**        | **CPU** | **Memory** |
|--------------------|--------|-----------|
| PostgreSQL (fiyopgdb) | 6 vCPU | 8 GB |
| MongoDB (fiyomgdb) | 4 vCPU | 6 GB |
| APIs (fiyoauth, fiyomain) | 6 vCPU each | 5 GB each |
| WebSockets (fiyochat) | 8 vCPU | 6 GB |
| RedisDB (fiyorsdb) | 2 vCPU | 4 GB |

## Cloudflare Free Plan

| **Service** | **Details** |
|------------|------------|
| CDN (fiyocdn) | Caching & delivery |
| Pages (fiyo) | Static site hosting |

## Wasabi Pay-as-You-Go

| **Service** | **Details** |
|------------|------------|
| Object Storage (fiyost) | 1TB, No extra fees |

## Predicted Latency

| **Service**        | **Predicted Latency** | **Notes** |
|--------------------|----------------------|----------|
| PostgreSQL        | **5-15 ms**           | Query execution depends on indexing and load. |
| MongoDB           | **5-20 ms**           | Read-heavy workloads may be faster; writes depend on replication. |
| APIs (fiyoauth, fiyomain) | **10-30 ms**   | Varies with concurrent requests and processing logic. |
| WebSockets (fiyochat) | **30-100 ms**     | Real-time but fluctuates under load due to shared resources. |
| RedisDB            | **1-5 ms**            | Low latency but depends on cache hit rate. |

This setup ensures balanced performance while keeping costs minimal. The shared infrastructure might introduce slight latency fluctuations, but overall, it remains optimized for real-time interactions.

