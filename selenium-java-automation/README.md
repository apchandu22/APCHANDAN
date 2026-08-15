# 🖥️ Selenium Java Automation — Sauce Demo Shopify

A practical UI automation project using **Selenium WebDriver + Java + TestNG + Maven + Page Object Model** for the demo e-commerce storefront:

urlSauce Demo Shopify Storehttps://sauce-demo.myshopify.com/

## 🎯 Objective

Demonstrate maintainable end-to-end web automation for an e-commerce application, including product navigation, product selection, cart validation and basic checkout navigation.

## 🛠️ Tech Stack

- Java
- Selenium WebDriver
- TestNG
- Maven
- Page Object Model (POM)
- WebDriverWait / Explicit Waits
- XPath / CSS Selectors
- Assertions
- Git / GitHub
- GitHub Actions

## 📂 Project Structure

```text
selenium-java-automation/
├── pom.xml
├── testng.xml
├── README.md
├── .gitignore
├── src/
│   └── test/
│       └── java/
│           └── com/chandan/automation/
│               ├── base/
│               │   └── BaseTest.java
│               ├── pages/
│               │   ├── HomePage.java
│               │   ├── ProductPage.java
│               │   └── CartPage.java
│               └── tests/
│                   └── EcommerceFlowTest.java
└── .github/
    └── workflows/
        └── selenium-tests.yml
```

## 🧪 Automated Coverage

| Test ID | Scenario | Type |
|---|---|---|
| AUTO-001 | Launch storefront and verify title | Smoke |
| AUTO-002 | Open product from storefront | Functional |
| AUTO-003 | Verify product details | Functional |
| AUTO-004 | Add product to cart | Functional |
| AUTO-005 | Verify cart contains selected product | Functional |
| AUTO-006 | Navigate toward checkout | E2E |

## 🏗️ Framework Design

The framework separates responsibilities using **Page Object Model**:

```text
Test Class
   ↓
Page Objects
   ↓
Reusable Locators / Actions
   ↓
Selenium WebDriver
   ↓
Browser
```

### Framework practices demonstrated

- Reusable page objects
- Centralized browser setup/teardown
- Explicit waits instead of hard sleeps
- Meaningful assertions
- Maven dependency management
- TestNG execution
- CI-ready project structure

## ▶️ Run Locally

### Prerequisites

- JDK 11+
- Maven 3.8+
- Chrome browser

### Execute tests

```bash
mvn clean test
```

### Execute TestNG suite

```bash
mvn test -DsuiteXmlFile=testng.xml
```

## ⚙️ CI/CD

GitHub Actions is configured to execute the Maven/TestNG suite on push and pull request events.

## ⚠️ Test Environment Note

This is a public demo storefront used for portfolio and learning purposes. UI selectors can change when the site changes. The automation code intentionally demonstrates maintainable locator and wait patterns rather than claiming production stability.

## 👨‍💻 Author

**A P Chandan** — Software Test Engineer | Manual Testing | API Testing | Selenium Java | GenAI for QA
