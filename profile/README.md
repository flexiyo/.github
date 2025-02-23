# How We Pay Only \$27 for Flexiyo 🚀

Building a powerful yet cost-effective cloud infrastructure for **Flexiyo** requires smart choices. We've optimized our setup using **Railway Pro for backend hosting, Wasabi for object storage, and Cloudflare for CDN and security**. Here’s a modern breakdown of our **monthly costs** and why this setup works best.

---

## 🚀 **Railway Pro (Backend Hosting & Databases)**

| Service                       | vCPU        | RAM       |
| ----------------------------- | ----------- | --------- |
| **PostgreSQL (fiyopgdb)**     | 6 vCPU      | 8 GB      |
| **MongoDB (fiyomgdb)**        | 4 vCPU      | 6 GB      |
| **APIs (fiyoauth, fiyomain)** | 6 vCPU each | 4 GB each |
| **WebSockets (fiyochat)**     | 8 vCPU      | 6 GB      |
| **RedisDB (fiyorsdb)**        | 2 vCPU      | 4 GB      |

✅ **Why Railway Pro?**

- **Fixed-cost backend** – Pro plan includes all backend services within \$20/month.
- **Balanced resource allocation** for optimal performance and cost-efficiency.

---

## 🌍 **Cloudflare (CDN & Static Web Hosting)**

| Service           | Features                              |
| ----------------- | ------------------------------------- |
| **CDN (fiyocdn)** | Global CDN, DDoS Protection, Free SSL |
| **Pages (fiyo)**  | Static Web Hosting                    |

✅ **Why Cloudflare?**

- **Free global CDN** speeds up content delivery while securing traffic.
- **Static hosting at zero cost**, avoiding unnecessary compute expenses.

---

## 💾 **Wasabi (Object Storage)**

| Service                     | Storage              |
| --------------------------- | -------------------- |
| **Object Storage (fiyost)** | 1TB (No egress fees) |

✅ **Why Wasabi?**

- **No egress or API fees**, making it **perfect for media storage**.
- **More affordable than AWS S3**, while maintaining high reliability.

---

## 💰 **Total Monthly Cost**

| Provider        | Cost (\$)   |
| --------------- | ----------- |
| **Railway Pro** | 20          |
| **Wasabi**      | 6.99        |
| **Cloudflare**  | 0           |
| **Total**       | **\$26.99** |

---

## 🔥 **Why This Setup Works?**

✅ **Scalable Backend** – Handles APIs, WebSockets, and databases efficiently.  
✅ **Cost-Effective Storage** – No hidden fees, predictable costs.  
✅ **Free CDN & Hosting** – Performance boost with no extra spending.  
✅ **Fixed Cost Strategy** – **Everything runs at just \$26.99/month**.  

---

## 🚀 **Conclusion**

For **just \$26.99 per month**, Flexiyo runs on a **high-performance, scalable, and cost-efficient infrastructure**. This **smart allocation** balances backend power, secure storage, and free CDN services.

**Want further optimizations or monitoring insights? Let’s discuss!** 😊

