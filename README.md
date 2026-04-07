# Telemetry Data Format Converter

## 📌 Project Overview

This project converts telemetry data from two different JSON formats into a unified standard format.

The system ensures that data from different sources can be processed consistently.

---

## 📂 Project Files

* `data-1.json` → Input Format 1
* `data-2.json` → Input Format 2
* `data-result.json` → Expected unified output
* `main.py` → Conversion logic and unit tests

---

## 🔄 Input Formats

### Format 1

* Contains flat structure
* Location stored as a single string ("/" separated)

### Format 2

* Nested structure
* Timestamp in ISO 8601 format
* Location fields separated

---

## 🎯 Output Format

Both formats are converted into:

* Standard device details
* Structured location object
* Unified data object
* Timestamp in milliseconds (epoch)

---

## ⚙️ Implementation Details

Two functions are implemented:

* `convertFromFormat1(jsonObject)`
* `convertFromFormat2(jsonObject)`

### Key Logic:

* Splitting location string into components
* Converting ISO timestamp → milliseconds
* Mapping fields to unified structure

---

## ▶️ How to Run

Make sure Python 3 is installed.

Run the following command:

```bash
python main.py
```

---

## ✅ Testing

* Unit tests are included using `unittest`
* Tests verify both formats produce correct output
* Successful run = all tests passed

---

## ⚠️ Notes

* Timestamp conversion is handled using `datetime`
* Ensure correct ISO format parsing
* Focus on test results (ignore extra console output)

---

## 🚀 Future Improvements

* Add support for more formats
* Add error handling
* Convert into API using Flask

---

## 👨‍💻 Author

Eshwar Thatikonda
