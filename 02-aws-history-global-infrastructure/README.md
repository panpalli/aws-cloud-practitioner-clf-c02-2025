# 📘 02 - AWS History & Global Infrastructure

This module summarises the evolution of AWS and the fundamentals of its global infrastructure, as covered in Stephane Maarek's CLF-C02 2025 course.

---

## 📜 AWS History

- **2002**: AWS began as an internal solution within Amazon.
- **2004**: First public service launched — **Amazon SQS**.
- **2006**: Launch of **S3** and **EC2** marked the start of AWS as we know it.
- Today, AWS powers major platforms like **Netflix**, **Dropbox**, **Airbnb**, **NASA**, and more.

---

## 💼 Market Leadership

- 📊 **2023 Revenue**: $90 billion  
- 📈 **2024 Q1 Market Share**: ~31% (vs. Microsoft Azure ~25%)
- 🥇 **13 years as leader** in Gartner’s Magic Quadrant
- 🌍 Over **1 million active customers**

---

## 🔧 What Can You Build on AWS?

- Websites and mobile backends
- Backup, storage, and enterprise infrastructure
- Big data processing
- Game servers, social apps, media streaming
- ➕ Practically **anything** scalable and reliable

---

## 🌐 AWS Global Infrastructure

### 🏁 1. Regions
- Independent clusters of data centers.
- Examples: `us-east-1` (Ohio), `ap-southeast-2` (Sydney)
- Most services are **region-scoped**.

### 🏢 2. Availability Zones (AZ)
- Each region contains 3–6 AZs (e.g., `ap-southeast-2a`, `2b`, `2c`).
- AZs are isolated from failures (redundant power/network).
- AZs are connected with **high bandwidth, low-latency links**.

### 🌍 3. Edge Locations
- 400+ Points of Presence (PoPs) in 90+ cities across 40+ countries.
- Power global services like **CloudFront** (CDN).
- Ensure **low-latency content delivery** to end users.

---

## 🎯 Choosing the Right AWS Region

Factors to consider:
1. **Compliance** – Data residency laws (e.g., France requires data to stay local)
2. **Latency** – Choose a region close to your users
3. **Service Availability** – Not all regions support all services
4. **Pricing** – Costs vary across regions

---

## 🌍 Global vs. Regional AWS Services

| Scope     | Examples                                 |
|-----------|------------------------------------------|
| Global    | IAM, Route 53, CloudFront, WAF           |
| Regional  | EC2, Lambda, Rekognition, Elastic Beanstalk |

---

## 💬 Reflection

> This section gave me a strong understanding of AWS's global scale and strategic considerations for designing cloud-based applications with resilience, speed, and compliance in mind.
