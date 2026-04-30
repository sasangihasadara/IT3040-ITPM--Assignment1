# IT3040 – Assignment 1 (Option 1)

## Playwright Automation Project – Sinhala Transliteration Testing

This project implements an automated testing solution for validating the Sinhala transliteration functionality available at:

🔗 https://www.pixelssuite.com/chat-translator

The automation script reads test cases from an Excel file, inputs Singlish text into the web application, captures the Sinhala output, compares it against expected results, and updates the Excel sheet with execution results.

---

## 📌 Objective

The main objective of this project is to:

* Automate functional testing of a web-based Sinhala transliteration system
* Validate correctness of outputs using predefined test cases
* Improve testing efficiency by eliminating manual validation

---

## ⚙️ Prerequisites

Ensure the following software is installed before running the project:

* Python 3.11 or 3.12
* Google Chrome (latest version recommended)
* Internet connection

---

## 📁 Project Setup

### 1. Extract the Project

Download and extract the project ZIP file to your local machine.

Example location:

```
E:\test_automation\test_automation
```

---

### 2. Navigate to Project Directory

Open Command Prompt and run:

```
cd /d E:\test_automation\test_automation
```

---

## 📦 Install Dependencies (One-Time Setup)

Run the following commands:

```
pip install -U pip
pip install playwright openpyxl
playwright install
```

---

## 📊 Prepare Test Data (Excel File)

Open the Excel file:

```
Assignment 1 - Test cases.xlsx
```

Fill ONLY the following columns:

* TC ID
* Input length type
* Input
* Expected output

⚠️ Important:

* Do NOT fill:

  * Actual output
  * Status

These will be automatically updated by the script.

---

## ▶️ Run the Automation Script

Execute the following command:

```
python test_automation.py --excel "Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
```

---

## 📈 Output & Results

After execution:

1. Open the Excel file
2. Verify the following columns are updated automatically:

   * Actual output
   * Status (Pass / Fail)

---

## 📝 Final Manual Update (Assignment Requirement)

After reviewing results, add TWO additional columns:

* Singlish input types covered
* Evidence / rationale for input coverage

Provide explanations based on your testing observations.

---

## 🗂️ Project Structure

```
test_automation/
│── test_automation.py
│── Assignment 1 - Test cases.xlsx
│── README.md
```

---

## ⚠️ Important Notes

* Ensure the Excel file is CLOSED before running the script
* Do NOT rename project files
* Maintain a stable internet connection
* Adjust delay parameters if necessary for slower systems

---

## 🚀 Features

* Automated input handling using Playwright
* Data-driven testing using Excel
* Real-time result validation
* Automatic result logging
* Configurable execution parameters

---

## 👨‍🎓 Author

**Student Registration Number:** IT23616738

---

## ✅ Conclusion

This project demonstrates how automated testing can be effectively applied to validate language processing systems, improving both accuracy and efficiency compared to manual testing approaches.

---
