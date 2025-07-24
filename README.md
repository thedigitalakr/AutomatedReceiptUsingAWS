# 🧾 Automated Receipt Extractor using AWS

This project automates the process of extracting data from uploaded receipts and notifying users via email. Built using AWS services: **S3, Lambda, Textract, DynamoDB, and SES**.

---

##  Project Overview

### Workflow:
1. User uploads a receipt image to an S3 bucket (`incoming/` folder).
2. A Lambda function is triggered by this upload.
3. The Lambda function uses **Amazon Textract** to extract data from the image.
4. Extracted data is stored in a **DynamoDB** table.
5. A confirmation email with receipt details is sent using **Amazon SES**.

---

## AWS Services Used

| Service     | Purpose                                      |
|-------------|----------------------------------------------|
| **S3**      | Stores receipt images                        |
| **Lambda**  | Extracts text and triggers actions           |
| **Textract**| OCR for structured/unstructured data         |
| **DynamoDB**| Stores structured receipt data               |
| **SES**     | Sends email notifications                    |
| **IAM**     | Grants secure permissions to Lambda, etc.    |

---
## Note
📌 Note: This project was built on AWS Free Tier and is no longer actively hosted. Screenshots and explanation are provided for demonstration purposes.
