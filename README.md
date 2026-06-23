# 📊 Automated Data Extraction & QA Pipeline using Python, OCR, and Regex

![Python](https://img.shields.io/badge/Python-3.x-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green)
![OCR](https://img.shields.io/badge/OCR-Tesseract-orange)
![Regex](https://img.shields.io/badge/Regex-Pattern%20Matching-red)
![Testing](https://img.shields.io/badge/Testing-Pytest-yellow)
## 📌 Overview

An automated **Data Quality Assurance and Document Intelligence system** built using Python, FastAPI, OCR, and data processing techniques.

This project focuses on transforming unstructured documents into accurate, structured, and validated data.

It simulates real-world Data QA workflows involving:

- Data extraction
- Data cleaning
- Data validation
- Pattern matching
- Quality testing
- Structured data generation


---

# 🎯 Business Problem

Healthcare organizations receive large amounts of unstructured medical documents such as:

- Patient information forms
- Prescription documents
- Medical records
- Healthcare reports

Manually processing these documents creates challenges:

❌ Data entry errors  
❌ Missing information  
❌ Inconsistent formatting  
❌ Slow processing time  

This project automates document processing by extracting, cleaning, and validating important medical information from unstructured PDF documents.
---

# 🚀 Key Features

## ✅ Automated Data Extraction

Extracts important information from PDF documents using OCR technology.

Example:

Raw document:

```
Name: Marta Sharapova

Address: New Russia

Refill: 3 times
```

Converted into structured data:

```json
{
    "patient_name": "Marta Sharapova",
    "address": "New Russia",
    "refills": "3"
}
```


---

## ✅ Data Cleaning Pipeline

The system improves raw document quality using:

- Image preprocessing
- Noise reduction
- Text normalization
- Pattern extraction


---

## ✅ Regex Based Validation

Uses regular expressions for accurate extraction of:

- Names
- Addresses
- Dates
- Phone numbers
- Numeric fields


---

## ✅ Data Quality Testing

Automated validation using Pytest.

Testing includes:

✔ Correct extraction  
✔ Missing value handling  
✔ Multiple document formats  
✔ Data accuracy checks  


---

# 🏗️ System Architecture

```
                User Uploads Document

                        |

                        ↓

                 FastAPI Endpoint

                        |

                        ↓

              PDF → Image Conversion

                        |

                        ↓

              Image Preprocessing

                        |

                        ↓

                  OCR Extraction

                        |

                        ↓

                Data Cleaning Layer

                        |

                        ↓

              Regex Validation Rules

                        |

                        ↓

              Structured JSON Output
```


---

# 🛠️ Technology Stack

## Programming

- Python


## Backend

- FastAPI


## Data Processing

- OpenCV
- NumPy


## OCR

- Tesseract OCR
- Pytesseract


## Testing

- Pytest


---

# 📂 Project Structure

```
medical-document-parser

│
├── backend
│
│   ├── src
│   │
│   │   ├── main.py
│   │   ├── extractor.py
│   │   ├── util.py
│   │   ├── parser_generic.py
│   │   ├── parser_prescription.py
│   │   └── parser_patient_details.py
│   │
│   ├── tests
│   │
│   │   ├── test_prescription_parser.py
│   │   └── test_patient_details_parser.py
│   │
│   └── docs
│
├── requirements.txt
│
├── README.md
│
└── .gitignore
```


---

# ⚙️ Installation

Clone repository:

```bash
git clone https://github.com/Maaz-05/medical_document_parser.git
```


Move into project:

```bash
cd intelligent-data-extraction-pipeline
```


Create virtual environment:

```bash
python -m venv .venv
```


Activate environment:

Windows:

```bash
.venv\Scripts\activate
```


Install dependencies:

```bash
pip install -r requirements.txt
```


---

# ▶️ Running Application

Start FastAPI server:

```bash
python backend/src/main.py
```


Open:

```
http://127.0.0.1:8000/docs
```


---

# 📌 API Workflow

Endpoint:

```
POST /extract_from_doc
```


Input:

```
file_format = prescription

file = document.pdf
```


Output:

```json
{
    "patient_name": "Marta Sharapova",
    "medicines": "Prednisone 20 mg",
    "directions": "Take daily",
    "refills": "3"
}
```


---

# 🧪 Running Tests

Run:

```bash
pytest
```


Test coverage:

- Extraction accuracy
- Data validation
- Missing values
- Multiple document cases


---

# 📈 Data QA Skills Demonstrated

This project demonstrates practical experience with:

✅ Data cleaning  
✅ Data labeling concepts  
✅ Data validation  
✅ Regex pattern matching  
✅ Unstructured data processing  
✅ Quality assurance testing  
✅ Python automation  
✅ Error handling  
✅ Structured data transformation  


---

# 🔮 Future Improvements

- Machine Learning based entity extraction
- Data quality dashboard
- Data anomaly detection
- Database integration
- Cloud deployment
- Automated reporting


---

# 👨‍💻 Author

**Maaz**

LinkedIn:
https://www.linkedin.com/in/maaz-ahmad-9b1aa7325/

