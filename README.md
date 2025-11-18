# 🛵 Scooter – Full End-to-End QA Project

Comprehensive QA project covering Web Testing, Mobile Testing, API Testing, SQL Validation, and Automation for the Scooter application.

---

## 📌 Scope
- Web Testing  
- API Testing (Postman)  
- SQL Validation  
- Mobile Testing  
- Automation (Pytest + Selenium)  
- Exploratory Testing  
- Documentation & Reporting  

---

## 📂 Project Structure

scooter-e2e-testing/
│
├── README.md
├── web-tests/
│ ├── ui-test-cases.xlsx
│ └── bug-reports.pdf
│
├── api-tests/
│ ├── postman-collection.json
│ └── automation/
│ ├── test_api_orders.py
│
├── mobile-tests/
│ └── emulator-recordings/
│
├── sql/
│ └── scooter-db-queries.sql
│
└── automation/
├── test_login.py
├── test_routes.py
└── conftest.py


---

## 🧪 Selenium Example

```python
from selenium import webdriver

def test_login_success():
    driver = webdriver.Chrome()
    driver.get("https://scooter-app.com/login")

    driver.find_element("id","email").send_keys("test@test.com")
    driver.find_element("id","password").send_keys("123456")

    driver.find_element("id","login-btn").click()

    assert "dashboard" in driver.current_url
    driver.quit()
🛠 Tools

Selenium WebDriver

Pytest

SQL

Postman

Android Studio

Git

👩‍💻 Author

Anyelly Natalia Flórez
QA Engineer — Manual & Automation
