# How We Run Flexiyo for Just ₹2000/Month

At **Flexiyo**, we prioritize cost-efficiency without compromising performance. Many developers assume that running a scalable API + AI + database infrastructure requires a massive budget, but we manage to keep our total cost at just **₹2000/month (€21.54/month)** while delivering **sub-50ms API responses** and efficient AI-powered recommendations.

## Our Optimized VPS Setup
To balance **performance, storage, and scalability**, we merged key services and optimized resource allocation. Here’s our final infrastructure setup:

### **🖥 VPS 1: Databases + APIs** (PostgreSQL + MongoDB + Node.js APIs)
- **Specs:**
  - ⚙️ **6 vCPU, 12GB RAM, 150GB NVMe SSD**
  - 🌐 **32TB Out + Unlimited In Bandwidth**
  - ⚡ **400 Mbit/s Connection**
- **Cost:** 💰 **€11.31/month (~₹1050/month)**
- **Why?**
  - ✅ **Merging APIs and databases eliminates network overhead**.
  - ✅ **6 vCPUs ensure high API throughput (~7,000 RPS)**.
  - ✅ **12GB RAM for optimized query execution**.
  - ✅ **NVMe SSD enhances indexing and read/write speeds**.
  - ✅ **High bandwidth ensures smooth operations under heavy traffic**.

### **🤖 VPS 2: AI + Object Storage + Brokers + Notifications** (TensorFlow + MinIO + RabbitMQ)
- **Specs:**
  - ⚙️ **4 vCPU, 4GB RAM, 100GB NVMe SSD**
  - 📂 **250GB Object Storage**
  - 🌐 **32TB Out + Unlimited In Bandwidth**
  - ⚡ **200 Mbit/s Connection**
- **Cost:** 💰 **€8.92/month (~₹830/month)**
- **Why?**
  - ✅ **4 vCPU handles AI inference, messaging, and storage efficiently**.
  - ✅ **250GB Object Storage for media files and AI data**.
  - ✅ **RabbitMQ ensures real-time notifications**.
  - ✅ **Optimized SSD storage for AI workload and recommendation systems**.
  - ✅ **High bandwidth to handle AI processing and real-time data streaming**.

### **🌍 Web Hosting** (Frontend + CDN)
- **Specs:**
  - 🏗 **100 Websites**
  - 📧 **100 Emails**
  - 📂 **100GB NVMe SSD**
- **Cost:** 💰 **€1.31/month (~₹120/month)**
- **Why?**
  - ✅ **Handles web traffic efficiently with static file caching**.
  - ✅ **Integrated CDN improves global load speeds**.
  - ✅ **Minimal cost while delivering fast website performance**.

## 📊 Performance Gains

| **Metric**                 | **Before** (Lower Specs) | **After** (Optimized Setup) |
|----------------------------|-----------------|-----------------|
| ⏱ **API Response Time**      | 50-60ms        | **30-40ms**     |
| ⚡ **Feed Loading Time**      | 900ms - 1s     | **700-900ms**   |
| 📊 **DB Query Time**          | 40-100ms       | **20-60ms**     |
| 🧠 **AI Inference Latency**   | 300-400ms      | **180-280ms**   |
| 🔥 **Peak Load Handling**     | ~5,000 RPS     | **~7,000 RPS**  |

## 🎯 Why This Works for Us
- 🔄 **API + DB Merged for Locality** → Eliminating external API-DB calls **reduces response times significantly**.
- ⚡ **Balanced Compute Allocation** → More **vCPUs for API & DB** ensures **fast query processing**.
- 🤖 **Optimized AI Workload** → AI inference runs smoothly **without over-provisioning**.
- 🌐 **Efficient Web Hosting** → Using a separate VPS for the frontend **improves speed and stability**.
- 💰 **Cost-Effective Scaling** → Instead of overpaying, we **pay only for what’s necessary**.
- 🚀 **High Bandwidth Allocation** → **32TB Out + Unlimited In** ensures smooth operations even under high traffic.

## 💰 Total Cost Breakdown (₹2000/month)

| VPS Role | Cost (€) | Cost (₹) |
|----------|----------|----------|
| 🖥 **VPS 1: Databases + APIs** (6 vCPU, 12GB RAM, 150GB SSD, 32TB Out) | **€11.31/mo** | **~₹1050/mo** |
| 🤖 **VPS 2: AI + Brokers + Storage** (4 vCPU, 4GB RAM, 250GB Object Storage, 100GB SSD, 32TB Out) | **€8.92/mo** | **~₹830/mo** |
| 🌍 **Web Hosting** (100 Websites, 100 Emails, 100GB NVMe) | **€1.31/mo** | **~₹120/mo** |
| **Total Cost** | **€21.54/mo** | **~₹2000/mo** |

---

💡 **Want to build a cost-effective, scalable architecture like ours?**  
Let us know in the comments or reach out! 🚀

