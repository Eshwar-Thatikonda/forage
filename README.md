# 🚀 Telemetry Data Format Converter

## 📌 Overview

A Python-based data normalization system that converts telemetry data from multiple heterogeneous JSON formats into a unified, structured format.

This project simulates real-world data engineering challenges where data arrives in inconsistent schemas and must be standardized for downstream processing.

---

## 🎯 Problem Statement

Different telemetry sources produce data in varying formats:

* Flat vs nested JSON structures
* Different timestamp formats (epoch vs ISO 8601)
* Inconsistent location representation

This project solves the problem by transforming all inputs into a single consistent schema.

---

## 🧠 Key Features

* 🔄 Multi-format JSON handling
* ⏱️ ISO 8601 → Epoch timestamp conversion (milliseconds)
* 📍 Structured location parsing
* 🧪 Automated unit testing using `unittest`
* ⚡ Clean and modular Python implementation

---

## 🏗️ Project Structure

```
├── data-1.json        # Input Format 1 (flat structure)
├── data-2.json        # Input Format 2 (nested structure)
├── data-result.json   # Expected unified output
├── main.py            # Core logic + unit tests
```

---

## 🔄 Data Transformation Logic

### ✅ Format 1 → Unified Format

* Splits location string into structured fields
* Maps:

  * `operationStatus → status`
  * `temp → temperature`

### ✅ Format 2 → Unified Format

* Extracts nested device information
* Converts ISO timestamp → milliseconds since epoch
* Direct mapping of structured location fields

---

## 🧪 Testing

This project uses Python's built-in `unittest` framework.

### ✔ Test Coverage:

* Format 1 conversion
* Format 2 conversion
* Output validation against expected result

---

## ▶️ How to Run

### 🔧 Prerequisites

* Python 3.x

### ▶ Run the project:

```bash
python main.py
```

### ✅ Expected Output:

All test cases should pass:

```
OK
```

---

## ⚙️ Technologies Used

* Python 3
* JSON Processing
* datetime module
* unittest framework

---

## 💡 Key Concepts Demonstrated

* Data normalization
* Schema transformation
* Timestamp conversion
* Test-driven validation
* Clean code practices

---

## 🚀 Future Enhancements

* Add support for additional telemetry formats
* Build REST API using Flask/Django
* Integrate with real-time data pipelines (Kafka)
* Add logging & error handling

---

## 📌 Real-World Applications

* IoT data processing systems
* Data engineering pipelines
* ETL (Extract, Transform, Load) workflows
* Monitoring and analytics platforms

---

## 👨‍💻 Author

**Eshwar Thatikonda**

* Passionate about Data Engineering & Backend Development
* Skilled in Python, Machine Learning, and System Design

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
