# 🚀 End-to-End Quality Intelligence Framework (QE 1.0)

> **Production-grade Quality Engineering framework that goes beyond automation to deliver real-time release quality intelligence using CI/CD, Allure dashboards, and Go/No-Go decision support.**

---

## 📌 Overview

The **End-to-End Quality Intelligence Framework** is a **QE 1.0-level automation and quality visibility platform** built by evolving a full-stack automation framework into a **decision-driven quality system**.

Unlike traditional automation frameworks that stop at *test execution*, this framework provides:

* **Smoke & Regression suite intelligence**
* **Critical test impact analysis**
* **Centralized Allure dashboards**
* **Release-level Go / No-Go visibility**
* **CI/CD-driven quality reporting**

This mirrors how **modern product companies** implement Quality Engineering.

---

## 🔥 Live Allure Quality Dashboard

📊 **Live Report (GitHub Pages)**
🔗 **[https://debasish-87.github.io/End-to-End-Quality-Intelligence-Framework/](https://debasish-87.github.io/End-to-End-Quality-Intelligence-Framework/)**

The dashboard is automatically generated and published on every pipeline run.

---

## 🧠 What Makes This a “Quality Intelligence” Framework?

Traditional automation answers:

> “Did tests pass?”

This framework answers:

> **“Is this build safe to release?”**

### Key Intelligence Layers:

* Test criticality awareness
* Smoke vs Regression confidence
* Severity-based risk visibility
* CI/CD-driven release readiness

---

## ✅ Core Capabilities

### 🧪 Test Automation Coverage

| Layer               | Tools              |
| ------------------- | ------------------ |
| UI Automation       | Selenium WebDriver |
| API Automation      | RestAssured        |
| Database Validation | MySQL              |
| Test Runner         | TestNG             |
| Language            | Java 17            |

---

### 🚦 Suite Intelligence

| Suite      | Purpose                           |
| ---------- | --------------------------------- |
| Smoke      | Fast confidence on critical flows |
| Regression | Full functional coverage          |
| Critical   | Business-blocking validations     |

Suites are controlled using:

* `smoke.xml`
* `regression.xml`
* TestNG groups (`Smoke`, `Regression`, `Critical`)

---

### 📊 Quality Metrics Engine

Automatically computes:

* Total tests executed
* Pass / Fail percentage
* Critical test failures
* Execution trends (Allure history ready)

---

### 🧠 Release Decision Engine

Generates decision-oriented insights like:

```
SMOKE: PASS
REGRESSION: 95%
CRITICAL FAILURES: 1

FINAL RELEASE DECISION: ❌ HOLD
```

This simulates **real release review meetings** in companies.

---

## 🏗️ Architecture Overview

```
Code Commit
   ↓
CI/CD Pipeline (GitHub Actions)
   ↓
Build + Test Execution
   ↓
Quality Intelligence Framework
   ├── UI Automation
   ├── API Automation
   ├── Database Validation
   ├── Smoke / Regression Suites
   ├── Critical Test Analysis
   ↓
Quality Metrics Engine
   ↓
Allure Centralized Dashboard
   ↓
Release Visibility (Go / No-Go)
```

---

## 🧩 Project Structure

```
End-to-End-Quality-Intelligence-Framework
│
├── pom.xml
├── README.md
├── testng.xml
├── smoke.xml
├── regression.xml
│
├── src
│   ├── main
│   │   ├── java
│   │   │   ├── base
│   │   │   │   ├── BaseTest.java
│   │   │   │   └── DriverManager.java
│   │   │   │
│   │   │   ├── pages
│   │   │   │   ├── LoginPage.java
│   │   │   │   ├── InventoryPage.java
│   │   │   │   └── CheckoutFlow pages
│   │   │   │
│   │   │   ├── intelligence
│   │   │   │   ├── metrics
│   │   │   │   │   ├── QualityMetrics.java
│   │   │   │   │   ├── AllureResultReader.java
│   │   │   │   │   └── CriticalTestAnalyzer.java
│   │   │   │   │
│   │   │   │   └── decision
│   │   │   │       └── ReleaseDecisionEngine.java
│   │   │   │
│   │   │   ├── api
│   │   │   └── utils
│   │   │
│   │   └── resources
│   │       ├── config.properties
│   │       ├── environment.properties
│   │       └── log4j2.xml
│   │
│   └── test
│       ├── java
│       │   ├── tests
│       │   │   ├── ui
│       │   │   └── api
│       │   │
│       │   └── intelligence
│       │       ├── QualityMetricsTest.java
│       │       └── ReleaseDecisionTest.java
│       │
│       └── resources
│           ├── testdata
│           └── categories.json
│
├── logs
├── allure-results
└── .github/workflows
    └── allure-deploy.yml
```

---

## 🧪 Test Execution Commands

### Run All Tests

```bash
mvn clean test
```

### Run Smoke Suite

```bash
mvn clean test "-DsuiteXmlFile=smoke.xml"
```

### Run Regression Suite

```bash
mvn clean test "-DsuiteXmlFile=regression.xml"
```

### Headless Mode (CI/CD)

```bash
mvn clean test -Dheadless=true
```

---

## 📊 Allure Reporting

### Generate & View Locally

```bash
mvn allure:serve
```

### Auto-Published via CI/CD

Allure reports are automatically:

* Generated after test execution
* Deployed to GitHub Pages
* Available as a live dashboard

---

## 🔁 CI/CD Pipeline (GitHub Actions)

The pipeline automatically:

* Runs on every push
* Executes tests
* Generates Allure reports
* Publishes reports to GitHub Pages

Workflow file:

```
.github/workflows/allure-deploy.yml
```

---

## 🧠 How to Explain This in an Interview

> “I built an End-to-End Quality Intelligence Framework that integrates UI, API, and database automation with CI/CD pipelines. It generates Allure dashboards and provides release-level quality visibility, enabling Go/No-Go decisions based on test criticality.”

🔥 This demonstrates **QE mindset**, not just automation.

---

## 🎯 Who Is This Framework For?

This project reflects **real-world Quality Engineering practices** used in:

* Product companies
* SaaS platforms
* Enterprise QE teams

Designed for:

* Scalable automation
* CI/CD integration
* Release confidence
* Stakeholder visibility

---

## 👤 Author

**Debasish**
SDET | QA Automation | Quality Engineering | CI/CD
📧 Email: [debasishm8765@gmail.com](mailto:debasishm8765@gmail.com)
🔗 GitHub: [https://github.com/Debasish-87](https://github.com/Debasish-87)

---
