# 🛒 AI-Powered E-Commerce Platform  
**Full-Stack | Spring Boot | React | Generative AI | Embeddings | pgvector**

---

## 📘 Executive Summary
The **AI-Powered E-Commerce Platform** is a full-stack application that integrates traditional e-commerce functionality with modern **AI-driven intelligence**.  
It combines a **Spring Boot backend** and a **React frontend** to deliver automated product content generation, semantic search, and an AI-powered shopping assistant.

The platform leverages **Generative AI**, **vector embeddings**, and **PostgreSQL (pgvector)** to improve product discovery, automate seller workflows, and enhance customer experience in a production-ready architecture.

---

## 🎯 Project Objectives
- Build a real-world **AI-enabled e-commerce platform**
- Automate **product description and image generation**
- Enable **semantic search and recommendations** using embeddings
- Implement an **AI shopping assistant** connected to live order and product data
- Design scalable and maintainable **REST APIs**

---

## 🚀 Key Features

### 🧠 AI Capabilities
- **AI-Generated Product Descriptions**  
  Automatically generates high-quality, brand-ready product descriptions using LLMs.

- **AI-Generated Product Images**  
  Generates realistic product images from product metadata without manual uploads.

- **Semantic Search with Embeddings + pgvector**  
  - Product data is converted into vector embeddings  
  - Stored in PostgreSQL using **pgvector**  
  - Enables context-aware product discovery beyond keyword search

- **AI Shopping Assistant (Chatbot)**  
  - Answers order-related questions  
  - Retrieves order history and order status  
  - Recommends products using vector similarity and user intent

---

### 🛒 Core E-Commerce Features
- Product creation, update, and deletion
- Product image upload and retrieval
- Shopping cart and checkout flow
- Order placement and tracking
- Inventory and availability management
- Keyword + semantic product search
- Cross-origin frontend integration

---

## 🧱 System Architecture
The application follows a layered monolithic architecture with AI services integrated into the service layer:

1. **Frontend (React)** – User interface and AI interaction  
2. **Controller Layer** – REST endpoints  
3. **Service Layer** – Business logic and AI orchestration  
4. **Data Access Layer** – Spring Data JPA repositories  
5. **Database Layer** – PostgreSQL + pgvector  
6. **AI Layer** – LLMs, embeddings, image generation

---

## 🛠 Tech Stack

### Backend
- Java 21
- Spring Boot 3
- Spring Data JPA, Hibernate
- PostgreSQL
- pgvector
- Spring AI / LLM Integration
- Maven
- Docker

### Frontend
- React
- Vite
- Axios
- HTML, CSS

---

## 📦 Key Dependencies

### Backend
- spring-boot-starter-web  
- spring-boot-starter-data-jpa  
- postgresql  
- lombok  
- Spring AI / OpenAI integration  

### Frontend
- React  
- Axios  
- Vite  

---

## 🔗 API Overview

| Endpoint | Method | Description |
|--------|--------|-------------|
| `/api/products` | GET | Retrieve all products |
| `/api/product/{id}` | GET | Get product by ID |
| `/api/product` | POST | Create product |
| `/api/product/{id}` | PUT | Update product |
| `/api/product/{id}` | DELETE | Delete product |
| `/api/product/search` | GET | Keyword + semantic search |
| `/api/orders` | POST | Place order |
| `/api/orders/{id}` | GET | Get order details |
| `/api/chat` | POST | AI shopping assistant |

---

## 🧪 Installation & Setup

### 🔧 Backend (Spring Boot)

```bash
cd SpringEcomAI
export OPENAI_API_KEY=your_api_key_here
./mvnw spring-boot:run
