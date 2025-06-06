# 🧠 DocuVision-AI

**DocuVision-AI** is an intelligent document classification and redaction pipeline built to streamline and secure the handling of sensitive government forms. By combining the power of **AWS Textract**, **custom machine learning models**, and **explainable AI**, it automates document classification, entity recognition, and redaction workflows with precision and transparency.

The pipeline is designed for scalability and compliance, enabling agencies to reduce manual labor, enhance document security, and meet regulatory standards efficiently.

## 📌 Features

- 📄 **Automated Document Classification**:
  - Sorts large volumes of scanned forms by type (e.g., tax, immigration, legal)
  - Trained models for high-accuracy classification based on layout and content
  - Includes confidence scores and explainable AI insights

- 🕵️‍♂️ **Entity Recognition & Redaction**:
  - Detects sensitive PII/PHI using AWS Textract + custom NER models
  - Auto-redacts names, SSNs, addresses, etc., with visual overlays
  - Supports customizable redaction policies per agency

- 🧠 **Explainable AI**:
  - Interactive dashboard showing model decisions
  - Highlights key terms and layout features driving classification/redaction
  - Ensures human oversight and auditability

- 🔁 **Workflow Integration**:
  - Batch processing with parallel pipeline execution
  - JSON and PDF output formats with redaction layers
  - RESTful API for integration with external document management systems

- ☁️ **Cloud-Native & Scalable**:
  - Serverless deployment with AWS Lambda and Step Functions
  - S3 for storage, DynamoDB for metadata tracking
  - IAM-based role access and secure key management via AWS KMS

## 🛠️ Tech Stack

- **AI/ML**: Custom NER models (spaCy, Transformers), Explainable AI (LIME/SHAP)
- **OCR**: AWS Textract
- **Backend**: Python (FastAPI), AWS Lambda, Step Functions
- **Storage**: Amazon S3, DynamoDB
- **Security**: IAM, AWS KMS, HTTPS
- **DevOps**: Docker, Terraform, GitHub Actions

## 🚀 Getting Started

### Prerequisites

- AWS Account with Textract, Lambda, S3, Step Functions enabled
- Python 3.10+
- Docker & AWS CLI
- Git

### Clone & Deploy

```bash
git clone https://github.com/your-username/docuvision-ai.git
cd docuvision-ai
./deploy.sh  # or use the Terraform modules inside /infra
