# 🏢 HRM Dashboard E2E Testing with Selenium

![Selenium](https://img.shields.io/badge/-selenium-%2343B02A?style=for-the-badge&logo=selenium&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

## Project Overview
This repository contains End-to-End (E2E) automated UI testing for a Human Resource Management (HRM) dashboard. The project demonstrates advanced Selenium WebDriver skills, focusing on handling complex web elements such as dynamic dropdowns, file uploads, web tables, and explicit waits.

**Target Website:** [OrangeHRM Demo](https://opensource-demo.orangehrmlive.com/) - A widely used HR management system for testing purposes.

## Tech Stack
* **Testing Framework:** Pytest
* **Automation Tool:** Selenium WebDriver
* **Language:** Python
* **Design Pattern:** Page Object Model (POM) to ensure code reusability and maintainability.

## Test Scenarios Covered
The automation scripts validate the following core HR workflows:

### 1. Authentication (`test_login.py`)
- [x] Verify successful login with valid Admin credentials.
- [x] Verify error message handling for invalid credentials.
- [x] Verify logout functionality.

### 2. Employee Management (`test_employee.py`)
- [x] Navigate to the PIM (Product Information Management) module.
- [x] Add a new employee (Handling text boxes and file upload for profile picture).
- [x] Interact with dynamic dropdowns (e.g., selecting Job Title or Employment Status).

### 3. Data Validation (`test_data_table.py`)
- [x] Search for an existing employee in the web table.
- [x] Extract and assert data from specific rows and columns.
- [x] Verify successful deletion of an employee record.

## 📂 Project Structure
```text
selenium-hrm-dashboard-e2e/
├── pages/                # Page Object classes (e.g., login_page.py, dashboard_page.py)
├── tests/                # Test scripts using Pytest (*_test.py)
├── locators/             # CSS Selectors and XPaths
├── test_data/            # JSON or CSV files for data-driven testing
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```
## How to Run the Tests
1. Clone the repository:
> git clone [https://github.com/thiyada-kitt/selenium-hrm-dashboard-e2e.git](https://github.com/thiyada-kitt/selenium-hrm-dashboard-e2e.git)

> cd selenium-hrm-dashboard-e2e
2. Create a virtual environment (Optional but recommended):
> python -m venv venv

> source venv/bin/activate  # On Windows use: venv\Scripts\activate
3. Install dependencies:
> pip install -r requirements.txt
4. Run tests:
> pytest tests/ -v -s
