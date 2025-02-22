# How We Pay Only $27 for Flexiyo 🚀

Building a powerful yet cost-effective cloud infrastructure for **Flexiyo** requires smart choices. We've optimized our setup using **Railway for backend hosting, Wasabi for object storage, and Cloudflare for CDN and security**. Here’s a modern breakdown of our **monthly costs** and why this setup works best.  

---

## 🚀 **Railway (Backend Hosting & Databases)**

| Service  | Plan  | vCPU | RAM | Cost ($) |
|----------|-------|------|-----|----------|
| **PostgreSQL (fiyopgdb)** | Pro | 8 vCPU | 12 GB | Included |
| **MongoDB (fiyomgdb)** | Pro | 6 vCPU | 8 GB | Included |
| **APIs & WebSockets (fiyoauth, fiyomain, fiyochat)** | Pro | 6 vCPU each | 4 GB each | Included |
| **RedisDB (fiyorsdb)** | Hobby | 8 vCPU | 8 GB | Included |

✅ **Why Railway?**
- **Fixed-cost backend** – Pro plan includes all backend services within $20/month.
- **Redis fits in the free Hobby plan**, reducing database costs.

---

## 🌍 **Cloudflare (CDN & Static Web Hosting)**

| Service  | Plan  | Features | Cost ($) |
|----------|-------|----------|----------|
| **CDN (fiyocdn)** | Free | Global CDN, DDoS Protection, Free SSL | $0 |
| **Pages (fiyo)** | Free | Static Web Hosting | $0 |

✅ **Why Cloudflare?**
- **Free global CDN** speeds up content delivery while securing traffic.
- **Static hosting at zero cost**, avoiding unnecessary compute expenses.

---

## 💾 **Wasabi (Object Storage)**

| Service | Plan | Storage | Cost ($) |
|---------|------|---------|----------|
| **Object Storage (fiyost)** | Pay-as-you-go | 1TB (No egress fees) | $6.99 |

✅ **Why Wasabi?**
- **No egress or API fees**, making it **perfect for media storage**.
- **More affordable than AWS S3**, while maintaining high reliability.

---

## 💰 **Total Monthly Cost**

| Provider    | Cost ($)  |
|------------|----------|
| **Railway** | 20      |
| **Wasabi**  | 6.99    |
| **Cloudflare** | 0  |
| **Total**   | **$26.99** |

---

## 🔥 **Why This Setup Works?**
✅ **Scalable Backend** – Handles APIs, WebSockets, and databases efficiently.  
✅ **Cost-Effective Storage** – No hidden fees, predictable costs.  
✅ **Free CDN & Hosting** – Performance boost with no extra spending.  
✅ **Fixed Cost Strategy** – **Everything runs at just $26.99/month**.  

---

## 🚀 **Conclusion**
For **just $26.99 per month**, Flexiyo runs on a **high-performance, scalable, and cost-efficient infrastructure**. This **smart allocation** balances backend power, secure storage, and free CDN services.

**Want further optimizations or monitoring insights? Let’s discuss!** 😊

