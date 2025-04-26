
# 🚀 AWS Event-Driven Data Pipeline

This project showcases a fully serverless data pipeline using AWS services including S3, EventBridge, Step Functions, Glue Jobs, and SNS. It is designed to automate file ingestion, transformation, and notification workflows.

---

## 🧭 Architecture Overview

This pipeline performs the following steps:

1. 📥 File upload to **S3 bucket**
2. 🔔 Triggers **EventBridge Rule**
3. 🔁 Executes **Step Function**
4. ⚗️ Runs a **Step Job** and **AWS Glue Job**
5. 📢 Sends notification via **SNS** upon completion

---

## 🛠️ Tools & Technologies Used

**Amazon S3**, **EventBridge**, **Step Functions**, **Glue Job**, **SNS**, **IAM**, **Python**, **CloudWatch**

---

---

## 📬 Notification Flow

Upon successful transformation:
- Glue job triggers SNS topic
- Sends message to subscribed emails or endpoints

---

## 📌 Notes

- Ensure all IAM roles have correct permissions (S3 read/write, Glue execution, SNS publish)
- Setup CloudWatch for monitoring and error alerts
