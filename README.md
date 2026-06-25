 

# 🌾 AgriTalk – Smart Farmer Assistant

### Voice + Chat Based Bilingual (Marathi + English) AI System

### Built using Rasa, Vosk, React Native, Spring Boot & MySQL

---

## 🚀 Overview

AgriTalk is a smart digital assistant designed especially for farmers. It provides:

* **Voice-based chatbot** (Marathi & English)
* **Chat-based assistant**
* **Farm management: crops, fertilizers, expense tracking**
* **Weather, market price, crop advisory**
* **Farmer profile & multi-farm support**
* **Full mobile app (React Native)**
* **Backend APIs built using Spring Boot + Hibernate**
* **Intelligent NLP using Rasa (DIET) + Vosk Speech Recognition**

---

## 🏗️ Project Structure

```
AgriTalk/
│── agent/            → Rasa AI Assistant
│── backend/          → Spring Boot (REST API + MySQL)
│── frontend/         → React Native Mobile App
│── .github/          → GitHub workflows (optional)
│── README.md
│── .gitignore
```

---

## 🔥 Key Features

### 🗣️ **1. Voice Assistant**

* Speech-to-Text using **Vosk** (Offline / Free)
* Supports **Marathi + English**
* Converts user speech → text → Rasa NLU → response → displayed in app

### 💬 **2. Chat Assistant**

* Text-based chat through Rasa APIs
* Handles intent recognition, entities, farm queries
 

### 📒 **3. Farmer Notebook**

* Add farms
* Add crops
* Add activities
* Add expenses
* Track progress

### 🧠 **4. AI + NLP**

* Rasa DIET model for intent classification
* Lexical, syntactic, and character n-gram features
* Custom rules & stories
* Bilingual responses

### 🔐 **5. Authentication & Multi-Farmer**

* Each farmer has their own profile
* Each farmer maintains multiple farms
* Backend maintains user-level isolation

---

## 🛠️ Technology Stack

### 🎯 **AI / NLP**

| Technology                  | Purpose                                              |
| --------------------------- | ---------------------------------------------------- |
| **Rasa Open Source**        | NLP, NLU, intent classification, dialogue management |
| **DIET Classifier**         | BERT-like architecture for intents + entities        |
| **Vosk Speech Recognition** | Free offline Speech-to-Text (Marathi + English)      |
| **TTS Engine (Optional)**   | Convert bot reply → speech                           |

---

### 📱 **Frontend (Mobile App)**

| Tech                                 | Usage                           |
| ------------------------------------ | ------------------------------- |
| **React Native**                     | Mobile application              |
| **Expo / RN CLI**                    | Development environment         |
| **React Native Paper / Tailwind RN** | UI styling                      |
| **Axios**                            | API calls to Spring Boot / Rasa |

---

### 🖥️ **Backend**

| Tech                | Usage                                  |
| ------------------- | -------------------------------------- |
| **Spring Boot**     | APIs for farmers, farms, crops, logs   |
| **Hibernate / JPA** | ORM                                    |
| **MySQL**           | Relational DB for multi-farmer support |
| **JWT**             | Authentication                         |

---

### 🗄️ **Database**

* **MySQL** (Free, local, fast, stable)
* Supports multi-user isolation
* Farmers → Farms → Activities → Expenses

---

### ☁️ **Cloud / Deployment (Free Options)**

| Layer               | Free Platform                 |
| ------------------- | ----------------------------- |
| React Native App    | **Expo**                      |
| Backend Spring Boot | **Render** / **Railway**      |
| Rasa Server         | **Railway** (Free tier)       |
| MySQL DB            | **PlanetScale** / **Railway** |
| Code Repo           | **GitHub**                    |

---

## ⚙️ Installation & Setup Guide

### 1️⃣ Clone Repository

```
git clone https://github.com/your-username/Agritalk.git
cd Agritalk
```

---

## 2️⃣ Setup Rasa Agent

```
cd agent
python -m venv rasa-env
rasa-env\Scripts\activate
pip install -r requirements.txt
rasa train
rasa run --enable-api
```

---

## 3️⃣ Setup Spring Boot Backend

```
cd backend
mvn clean install
mvn spring-boot:run
```

Backend runs at:
👉 `http://localhost:8080`

---

## 4️⃣ Setup React Native App

```
cd frontend
npm install
npm start
```

If using Expo:
👉 Scan QR code from Expo Go app.

---

## 🧪 Testing Voice Bot

1. Start Rasa server
2. Frontend records audio
3. Vosk converts speech → text
4. Text is sent to Rasa API
5. Rasa generates reply
6. Reply is spoken using TTS (optional)

---

## 🚀 Future Enhancements

* Offline mode for farmers with poor network
* AI-based crop disease prediction
* WhatsApp chatbot integration
* On-device speech recognition tuning

---

## 👥 Stakeholders

* **Farmers (Primary Users)**
 
---
 