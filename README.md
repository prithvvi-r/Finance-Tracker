# 💰 AI-Powered Finance Tracker

An intelligent, modular finance tracking system built using **Spring Boot**, **LangChain**, **LLMs**, and **Kafka** — designed to automate expense management by extracting, categorizing, and analyzing transactions directly from SMS data.

---

## 🚀 Overview

The **AI-Powered Finance Tracker** eliminates manual expense entry by integrating **AI-based data extraction** from SMS messages.  
Using **LangChain** and **LLM APIs**, it processes messages intelligently, categorizes transactions automatically, and delivers analytics in real-time through a **microservice architecture**.

---

## 🧩 Architecture

This project follows a **microservice-based architecture**, ensuring scalability, fault-tolerance, and high performance.  
Each service operates independently and communicates via **Kafka** and **REST APIs**.

### Core Services
| Service | Description |
|----------|-------------|
| **Auth Service** | Handles user authentication and authorization using **JWT** tokens. |
| **User Service** | Manages user data, profiles, and linked financial accounts. |
| **DataScience Service (DS Service)** | Uses **LangChain** and **LLMs** to extract transaction details from SMS and categorize expenses automatically. |
| **Expense Service** | Maintains categorized expense records and analytics dashboards. |
| **Gateway (Kong)** | Manages routing, load balancing, and API security across microservices. |

---

## ⚙️ Tech Stack

| Category | Technologies |
|-----------|---------------|
| **Language** | Java |
| **Framework** | Spring Boot |
| **Build Tool** | Gradle |
| **AI/LLM Integration** | LangChain + External LLM API |
| **Data Pipeline** | Apache Kafka |
| **Database** | MySQL |
| **Containerization** | Docker |
| **API Gateway** | Kong |
| **Architecture** | Microservices |

---

## 🧠 AI & Automation

- **LangChain Integration**: Parses SMS data to extract merchant names, amounts, and timestamps.  
- **LLM-Powered Categorization**: Automatically classifies transactions (e.g., Food, Travel, Utilities).  
- **Smart Data Insights**: Generates spending summaries and pattern recognition.

---

## 📊 Achievements

- Automated **100% manual expense tracking** using LangChain and SMS parsing.  
- Improved processing speed by **80%** with Kafka handling **10,000+ transactions** concurrently.  
- Achieved **92% precision** in ML-based expense categorization.  
- Maintained **99.9% uptime** using Dockerized microservices and Kong Gateway.

---

## 🐳 Docker Setup

To run all services together:

```bash
# Build Docker images for all services
docker-compose build

# Start containers
docker-compose up


Ensure Kong, MySQL, and Kafka are properly configured in docker-compose.yml.

🔑 LLM API Configuration (DS Service)

The DataScience Service uses LangChain and an LLM API for intelligent SMS parsing.

Step 1: Create a .env file in dataservice/

OPENAI_API_KEY=your_api_key_here




🧩 This ensures your API key stays secure and never appears in version control.

📁 Repository Structure
finance-tracker/
│
├── authservice/
├── userservice/
├── dataservice/
│   ├── .env
│   └── src/main/resources/application.properties
├── expenseservice/
├── gateway/
├── docker-compose.yml
└── README.md

🔒 Security

JWT-based authentication for all secured routes.

Kong Gateway enforces rate limiting and API key validation.

Environment variables manage all sensitive credentials.

🧪 Future Enhancements

Integration with UPI/Bank APIs for real-time transactions.

Expense forecasting using ML models.

Web dashboard and mobile app support.

🧑‍💻 Author

Pruthviraj Pesode

Engineering Student | Java & Spring Boot Developer | AI Innovator
Building intelligent, scalable systems that automate human effort.

📧 Contact: [pruthvirajpesode@gmail.com]
🌐 GitHub: [github.com/prithvvi-r]

⭐️ Show Your Support

If you like this project, give it a ⭐ on GitHub — it motivates continuous innovation!

---

Would you like me to add **badges** (e.g., build passing, Docker ready, LangChain powered, Java version) and a **one-line tagline banner** at the top for a more polished GitHub profile presentation?
