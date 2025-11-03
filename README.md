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

### 🧩 Backend (AWS Lambda)

1. **Navigate to the backend folder:**
   ```bash
   cd backend
2.Install Dependencies
   ```bash
   pip install -r requirements.txt
3.Connect Lambda to API Gateway and create a new REST endpoint, e.g.:

/GetCollegeInfo

4.Ensure permissions:

Your Lambda execution role should allow access to Amazon S3 and AWS Bedrock.

5.Test the Lambda function using sample input from the AWS Console.
