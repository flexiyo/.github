# Running Flexiyo on a Lean ₹2000/Month Infrastructure

At **Flexiyo**, we’ve engineered a cost-efficient infrastructure that delivers reliable performance without straining our budget. While many assume scalable API, AI, and database systems demand significant investment, we operate at **₹2000/month (€21.54/month)**, achieving **sub-50ms API responses** and effective AI-driven recommendations.

## Our Infrastructure Setup
To optimize for performance, storage, and scalability, we’ve consolidated services and fine-tuned resource usage. Here’s how we’ve structured our systems:

### **🖥 VPS 1: Databases + APIs** (Contabo 6 vCPU Plan - PostgreSQL + MongoDB + Node.js APIs)
- **Specs:**
  - ⚙️ **6 vCPU, 12GB RAM, 150GB NVMe SSD**
  - 🌐 **32TB Outbound + Unlimited Inbound Bandwidth**
  - ⚡ **400 Mbit/s Connection**
- **Cost:** 💰 **€11.31/month (~₹1050/month)**
- **Rationale:**
  - Co-locating APIs and databases reduces network latency.
  - 6 vCPUs support high API throughput (~7,000 RPS).
  - 12GB RAM enables efficient query handling.
  - NVMe SSD boosts indexing and data access speeds.
  - Generous bandwidth accommodates traffic surges.

### **🤖 VPS 2: AI + Object Storage + Brokers + Notifications** (Contabo 4 vCPU Plan - TensorFlow + MinIO + RabbitMQ)
- **Specs:**
  - ⚙️ **4 vCPU, 4GB RAM, 100GB NVMe SSD**
  - 📂 **250GB Object Storage**
  - 🌐 **32TB Outbound + Unlimited Inbound Bandwidth**
  - ⚡ **200 Mbit/s Connection**
- **Cost:** 💰 **€8.92/month (~₹830/month)**
- **Rationale:**
  - 4 vCPUs manage AI inference, messaging, and storage workloads.
  - 250GB object storage supports media and AI data needs.
  - RabbitMQ facilitates real-time notifications.
  - NVMe SSD optimizes AI processing and recommendation tasks.
  - High bandwidth ensures seamless data streaming.

### **🌍 Web Hosting** (MilesWeb Elite Plan - Frontend + CDN)
- **Specs:**
  - 🏗 **100 Websites**
  - 📧 **100 Emails**
  - 📂 **100GB NVMe SSD**
- **Cost:** 💰 **€1.31/month (~₹120/month)**
- **Rationale:**
  - Efficiently manages web traffic with static file caching.
  - Integrated CDN enhances global load times.
  - Low-cost solution for stable frontend performance.

## 📊 Performance Outcomes

| **Metric**                 | **Before** (Lower Specs) | **After** (Current Setup) |
|----------------------------|--------------------------|---------------------------|
| ⏱ **API Response Time**      | 50-60ms                 | **30-40ms**              |
| ⚡ **Feed Loading Time**      | 900ms - 1s             | **700-900ms**            |
| 📊 **DB Query Time**          | 40-100ms                | **20-60ms**              |
| 🧠 **AI Inference Latency**   | 300-400ms               | **180-280ms**            |
| 🔥 **Peak Load Handling**     | ~5,000 RPS              | **~7,000 RPS**           |

## 🎯 Key Design Choices
- **API + DB Co-location**: Hosting APIs and databases together minimizes external call delays, improving response times.
- **Resource Balance**: Allocating more vCPUs to APIs and databases ensures quick query execution.
- **Lean AI Setup**: The AI workload runs efficiently without excessive resources.
- **Separate Web Hosting**: Isolating the frontend on MilesWeb’s Elite Plan enhances speed and reliability.
- **Cost Efficiency**: We provision only what’s needed, avoiding overpayment.
- **Bandwidth Capacity**: 32TB outbound and unlimited inbound bandwidth supports high-traffic scenarios.

## 💰 Total Cost Breakdown (₹2000/month)

| Component | Provider/Plan | Cost (€) | Cost (₹) |
|-----------|---------------|----------|----------|
| 🖥 **VPS 1: Databases + APIs** | Contabo (6 vCPU, 12GB RAM, 150GB SSD, 32TB Out) | **€11.31/mo** | **~₹1050/mo** |
| 🤖 **VPS 2: AI + Brokers + Storage** | Contabo (4 vCPU, 4GB RAM, 250GB Object Storage, 100GB SSD, 32TB Out) | **€8.92/mo** | **~₹830/mo** |
| 🌍 **Web Hosting** | MilesWeb Elite (100 Websites, 100 Emails, 100GB NVMe) | **€1.31/mo** | **~₹120/mo** |
| **Total Cost** | | **€21.54/mo** | **~₹2000/mo** |

---

💡 **Interested in building a lean, scalable system?**  
We’re happy to share insights—feel free to ask questions or reach out! 🚀
