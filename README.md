
# 🚖 Uber Simulation – Distributed Microservices Architecture

Welcome to a scalable, production-inspired simulation of the Uber ride-sharing platform.  
Designed as part of the **Distributed Systems for Data Engineering** course, this project demonstrates a robust microservices architecture using modern technologies: **Kafka, Docker, MySQL, MongoDB, Redis, and Machine Learning**.

This clone models real-world challenges including:
- Dynamic pricing under load
- High concurrency
- Geo-based driver matching
- Modular scalability using cloud-native principles

---

## 🧱 System Architecture

```plaintext
Frontend (React / Node.js)
        ↓
REST APIs (Express Microservices)
        ↓
Kafka Broker ↔ Redis Cache
        ↓
MySQL + MongoDB
````

Each backend service runs in isolation using **Docker** and communicates asynchronously via **Kafka**. The frontend interacts through REST APIs.

---

## 🧩 Key Features

* 🔁 **Microservices**: Drivers, Customers, Billing, Rides, and Admin
* 📦 **Kafka Messaging**: Asynchronous, event-driven communication
* 🧠 **Dynamic Pricing**: Machine Learning model for real-time pricing
* ⚡ **Redis Caching**: Improves performance by reducing DB hits
* 📍 **Location Matching**: Matches customers to nearby drivers
* 📷 **Media Uploads**: Videos/images for driver and customer interfaces
* 📊 **Admin Dashboard**: Real-time stats and revenue analytics

---

## 🔧 Tech Stack

| Layer     | Tools & Technologies                           |
| --------- | ---------------------------------------------- |
| Frontend  | Node.js, React.js                              |
| Backend   | Express.js, REST APIs, Kafka                   |
| Databases | MySQL (structured), MongoDB (media/data)       |
| Caching   | Redis                                          |
| ML Engine | Python, Scikit-learn                           |
| DevOps    | Docker, Docker Compose, JMeter, GitHub Actions |

---

## 🚀 Quick Start (With Docker)

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/Uber_Rides.git
cd Uber_Rides

# 2. Build and launch all services
docker-compose up --build -d

# 3. (Optional) View logs to ensure all services are running
docker-compose logs -f

# 4. Start frontend locally
cd frontend
npm install
npm run dev
```

> ✅ **Make sure Docker is running** before starting the services.

---

## 📈 Performance & Scalability

Tested using **Apache JMeter** under various configurations:

| Configuration   | Throughput ↑ | Latency ↓ |
| --------------- | ------------ | --------- |
| B (Base)        | Moderate     | Moderate  |
| B + SQL Caching | High         | Low       |
| B + S + Kafka   | Higher       | Lower     |
| B + S + K + Opt | Highest      | Lowest    |

---

## 🖼️ Screenshots

### 🚘 Uber Hero Section
<img src="https://github.com/user-attachments/assets/5121c425-3aed-4947-bcac-191fd41ee860" width="100%" alt="Uber Hero Section" />

### 🙌 Why Choose Us
<img src="https://github.com/user-attachments/assets/b1cc3c4e-d4be-4707-bcaf-46e46fe97c60" width="100%" alt="Why Choose Us Section" />


## ✅ Final Notes

This project reflects a real-world distributed system with:

* **Asynchronous communication**
* **Dynamic decision-making**
* **High availability**
* **Modular scalability**

It serves as a strong foundation for building production-level, cloud-native platforms.

⭐ Star this repo if you found it helpful or inspiring!


