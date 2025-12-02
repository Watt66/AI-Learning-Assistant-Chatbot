# AI-Learning-Assistant-Chatbot
# 📚 AI Learning Assistant Chatbot (LLM + Retrieval)

A simple, fully working chatbot that uses a Large Language Model (LLM) with document retrieval to provide context‑aware academic assistance.

This project is built using **Python**, **Flask**, and the **OpenAI API**.

---

## 🚀 Features

* Context‑aware answers using **OpenAI LLMs**
* Embedding‑based **document retrieval**
* Simple **Flask backend API**
* Easy to extend and deploy

---

## 📁 Project Structure

```
AI-Learning-Assistant/
│── app.py
│── requirements.txt
│── data/
│    └── docs.json
```

---

## 📦 Installation Guide

Follow the steps below to set up the project locally.

### **1. Clone the Repository**

```bash
git clone https://github.com/your-username/AI-Learning-Assistant.git
cd AI-Learning-Assistant
```

### **2. Create a Virtual Environment**

```bash
python -m venv venv
```

Activate it:

* **Windows:**

```bash
venv\Scripts\activate
```

* **macOS/Linux:**

```bash
source venv/bin/activate
```

### **3. Install Dependencies**

```bash
pip install -r requirements.txt
```

---

## 🔑 Set Your OpenAI API Key

You must set your API key as an environment variable.

### **Windows (PowerShell)**

```powershell
setx OPENAI_API_KEY "your-key-here"
```

### **macOS/Linux**

```bash
export OPENAI_API_KEY="your-key-here"
```

---

## 📝 Adding Study Documents

Edit the file:

```
data/docs.json
```

Example content:

```json
[
  {
    "title": "Python Basics",
    "content": "Python is a popular programming language used for automation, AI, backend development, and more."
  }
]
```

You may add multiple documents.

---

## ▶️ Running the Application

Start the Flask server:

```bash
python app.py
```

Server will run on:

```
http://127.0.0.1:5000
```

---

## 💬 Testing the Chatbot API

Use **curl**, Postman, or Thunder Client.

### Example Request:

```bash
curl -X POST http://127.0.0.1:5000/chat \
     -H "Content-Type: application/json" \
     -d "{\"query\": \"What is Python?\"}"
```

---

## ☁️ Uploading Your Project to GitHub

Run the following commands inside your project folder:

```bash
git init
git add .
git commit -m "Initial working AI Learning Assistant"
```

Connect to GitHub:

```bash
git remote add origin https://github.com/your-username/AI-Learning-Assistant.git
git branch -M main
git push -u origin main
```

Your project is now live on GitHub! 🎉

---

## 🙌 Credits

Built using:

* Python
* Flask
* OpenAI API

Feel free to extend this project with UI, vector databases, or advanced retrieval logic.
