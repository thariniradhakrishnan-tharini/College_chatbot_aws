# 🎓 College Chatbot using AWS Cloud

The **College Chatbot** is an intelligent assistant that provides instant answers to students’ college-related queries such as faculty details, project ideas, syllabus information, and FAQs.  
It uses **AWS Lambda**, **Amazon S3**, and **AWS Bedrock (Claude)** for backend processing, with a **React.js frontend** for a smooth chat experience.

---

## 🚀 Features
- Department-wise question answering (CSE, IT, ECE, etc.)
- Smart responses generated using **AWS Bedrock (Claude)**
- Data fetched from **Amazon S3** JSON files
- Clean and responsive chat interface built with **React**
- Chat history saved locally for each session

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

### 🧩 Backend (AWS Lambda)
1. Navigate to the backend folder:
   ```bash
   cd backend
