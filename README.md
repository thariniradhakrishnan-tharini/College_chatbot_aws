# 🎓 College Chatbot using AWS Cloud

The **College Chatbot** is an intelligent virtual assistant that provides instant answers to students’ college-related queries such as faculty details, project ideas, syllabus information, and FAQs.  
It leverages **AWS Lambda**, **Amazon S3**, and **AWS Bedrock (Claude)** for backend processing, with a **React.js frontend** for an interactive and responsive chat experience.

---

## 🚀 Features
- Department-wise question answering (CSE, IT, ECE, etc.)
- Smart responses generated using **AWS Bedrock (Claude)**
- Data fetched securely from **Amazon S3** JSON files
- Clean, fast, and mobile-friendly chat interface built with **React**
- Chat history stored locally for each user session
- Easy deployment via AWS Lambda + API Gateway

---

## 🧠 Tech Stack

| Layer | Technology |
|--------|-------------|
| **Frontend** | React.js |
| **Backend** | AWS Lambda (Python) |
| **Cloud Services** | Amazon S3, AWS Bedrock, API Gateway |
| **Database** | JSON files stored in S3 |
| **Hosting** | AWS Amplify / S3 static hosting |

---
## ⚙️ Setup Instructions

---

### 🧩 Backend (AWS Lambda)

1. **Navigate to the backend folder:**
   ```bash
   cd backend
---
2. **Install Dependencies**
    ```bash
    pip install -r requirements.txt
---
3. **Create env file and Add the below to the env file**
   ```bash
   touch .env
   
    REACT_APP_API_URL=https://your-api-gateway-url.amazonaws.com/prod/chat
---
4. **Start the development server**
    ```bash
    npm start
---
5. **Visit the app in your browser at**
    ```bash
    http://localhost:3000
---

### 🧩 FrontEnd (AWS Lambda)
1. **Move to the Folder**
   ```bash
   cd frontend
---
2. ** Install Reuirements**
   ```bash
   npm install
---
3. **Run the Program**
   ```bash
   npm run dev
---

## ⚡ Connection Overview

💬 **Frontend (React.js)**  
⬇️ Sends user queries via HTTP request  

🌐 **API Gateway**  
⬇️ Routes the request securely  

⚙️ **AWS Lambda (Python)**  
↳ Fetches data from **Amazon S3**  
↳ Calls **AWS Bedrock (Claude)** for intelligent responses  

📤 **Response → Returned to Frontend Chat UI**

---

✅ **How it works (explanation):**
- **Frontend (React)** → Sends user questions to API Gateway.  
- **API Gateway** → Routes requests securely to AWS Lambda.  
- **AWS Lambda** → Executes logic, fetches or generates answers using:  
  - **Amazon S3** → for static college data (faculty, syllabus, FAQs).  
  - **AWS Bedrock** → for AI-generated responses (Claude model).  
- Response is returned → displayed in the chat UI.

---

⚙️ **AWS Lambda (Python)**  
↳ Fetches data from **Amazon S3**  
↳ Calls **AWS Bedrock (Claude)** for intelligent responses  

📤 **Response** → Returned to **Frontend Chat UI**
