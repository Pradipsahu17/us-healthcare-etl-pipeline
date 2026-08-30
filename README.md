# US Healthcare Data ETL Project
## 📌 Project Overview

This project focuses on processing and transforming **US Healthcare data** using ETL (Extract, Transform, Load) processes.

The project currently contains three major healthcare data domains:

1. **Eligibility Data (`etl_elig`)**
2. **Medical Claims Data (`etl_med`)**
3. **Pharmacy Claims Data (`etl_rx_claims`)**

The objective is to load raw healthcare data, perform data validation and transformation, and prepare clean, structured data for analytics and reporting.

---

## 📂 Project Data Files

### 1. `etl_elig` – Eligibility Data

The `etl_elig` dataset contains member eligibility and demographic information.

Typical fields include:

* Member ID
* Member Name
* Date of Birth
* Gender
* Address
* ZIP Code
* SSN
* Relationship Code
* Medical/Insurance Coverage information
* Eligibility dates

**Purpose:**

* Identify covered members
* Track member eligibility periods
* Maintain demographic information
* Support enrollment and healthcare utilization analysis

---

### 2. `etl_med` – Medical Claims Data

The `etl_med` dataset contains **medical healthcare claim transactions**.

The data can be used to analyze healthcare services received by members and the associated claim costs.

Typical information includes:

* Member ID
* Claim ID
* Provider information
* Service dates
* Diagnosis information
* Procedure information
* Place of service
* Billed amount
* Allowed amount
* Paid amount
* Claim status

**Purpose:**

* Analyze medical utilization
* Calculate healthcare costs
* Analyze provider and service utilization
* Support medical claims reporting

---

### 3. `etl_rx_claims` – Pharmacy Claims Data

The `etl_rx_claims` dataset contains **pharmacy prescription claim information**.

Typical information includes:

* Member ID
* Claim ID
* Prescription information
* Drug/NDC information
* Pharmacy information
* Prescription/service date
* Quantity
* Days supply
* Paid amount
* Copay
* Claim status

**Purpose:**

* Analyze prescription utilization
* Track pharmacy claims
* Calculate pharmacy costs
* Support medication and drug utilization analysis

---

## 🔄 ETL Process

The overall ETL process follows these stages:

```text
Raw Healthcare Data
        │
        ▼
     Extract
        │
        ▼
   Data Validation
        │
        ▼
    Transform
        │
        ├──────────────┐
        ▼              ▼
   Eligibility    Medical Claims
    etl_elig         etl_med
        │
        └───────┐
                ▼
        Pharmacy Claims
         etl_rx_claims
                │
                ▼
       Clean / Structured Data
                │
                ▼
        Analytics & Reporting
```

---

## 🛠️ Technologies Used

* **PostgreSQL**
* **SQL**
* **ETL**
* **Data Validation**
* **Data Transformation**
* **Healthcare Data Analytics**

---

## 📊 Healthcare Data Domains

| Dataset         | Domain          | Primary Purpose                       |
| --------------- | --------------- | ------------------------------------- |
| `etl_elig`      | Eligibility     | Member enrollment and coverage        |
| `etl_med`       | Medical Claims  | Medical services and healthcare costs |
| `etl_rx_claims` | Pharmacy Claims | Prescription and pharmacy utilization |

---

## 🎯 Project Objectives

* Build an ETL pipeline for healthcare datasets
* Validate incoming healthcare data
* Transform raw data into structured datasets
* Maintain data quality and consistency
* Integrate eligibility, medical claims, and pharmacy claims data
* Prepare data for healthcare analytics and reporting

---

## 🔍 Data Quality Checks

The ETL process includes validation checks such as:

* Duplicate member/claim detection
* Missing value identification
* Date validation
* Invalid member ID detection
* Invalid claim records
* Amount validation
* Referential integrity checks
* Data type validation

---

## 📈 Potential Analytics

The processed datasets can be used to calculate healthcare metrics such as:

* Member enrollment
* Medical PMPM
* Pharmacy PMPM
* Total medical cost
* Total pharmacy cost
* Claim volume
* Member utilization
* Prescription utilization
* Provider utilization
* Healthcare cost trends

---

## 🚀 Future Enhancements

Future improvements may include:

* Automating the ETL pipeline
* Adding Python/Pandas processing
* Adding PySpark for large datasets
* Implementing incremental data loading
* Adding automated data-quality checks
* Creating healthcare analytics dashboards
* Implementing logging and error handling
* Adding AWS-based data processing

---

## 👨‍💻 Author

**Pradip Sahu**

Database / SQL Professional | ETL | Data Engineering

Interested in **Healthcare Data Analytics, Data Engineering, PostgreSQL, SQL, Python, and PySpark**.
