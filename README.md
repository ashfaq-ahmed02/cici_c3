# 🚀 C3 CI/CD — GitHub Actions Automation

<div align="center">

# ⚙️ C3 CI/CD

### Learn • Build • Automate • Deploy

A hands-on **CI/CD learning project** created for the **C3 – Campus to Corporate Club** to understand how modern software teams automate testing, building, and deployment using **GitHub Actions**.

<br>

![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge\&logo=github\&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge\&logo=github-actions\&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-Testing-0A9EDC?style=for-the-badge\&logo=pytest\&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI%2FCD-Automation-success?style=for-the-badge)

</div>

---

## 📌 About the Project

**C3 CI/CD** is a practical repository created to demonstrate the fundamentals of **Continuous Integration (CI)** and **Continuous Deployment (CD)** using GitHub Actions.

The project demonstrates how a developer can move from:

```text
Write Code
    ↓
Push to GitHub
    ↓
Automated Testing
    ↓
Build
    ↓
Create Artifact
    ↓
Deploy
```

Instead of manually performing repetitive tasks, GitHub Actions can execute them automatically whenever changes are pushed.

This repository is designed as a **beginner-friendly DevOps and CI/CD learning project** for students and members of C3.

---

# 🎯 Objectives

This project demonstrates:

| Concept                   | Purpose                             |
| ------------------------- | ----------------------------------- |
| 🔄 Continuous Integration | Automatically validate code changes |
| 🧪 Automated Testing      | Run tests using Pytest              |
| ⚙️ GitHub Actions         | Automate development workflows      |
| 🏗️ Build Automation      | Generate deployable artifacts       |
| 🚀 Continuous Deployment  | Deploy through GitHub Pages         |
| 🔗 Job Dependencies       | Connect CI → Build → Deploy         |
| 🤖 DevOps Automation      | Reduce repetitive manual work       |

---

# 🧠 What is CI/CD?

## 🔵 Continuous Integration

**Continuous Integration (CI)** means automatically checking and testing code whenever developers push changes.

Without CI:

```text
Developer
    ↓
Write Code
    ↓
Push Code
    ↓
Remember to Test Manually
    ↓
Find Problems Later
```

With CI:

```text
Developer
    ↓
git push
    ↓
GitHub
    ↓
GitHub Actions
    ↓
Automated Tests
    ↓
✅ Pass / ❌ Fail
```

In this repository, GitHub Actions automatically installs Python and Pytest and runs the test suite.

---

## 🟢 Continuous Deployment

**Continuous Deployment (CD)** means automatically deploying software after the required checks and build stages succeed.

The workflow in this project follows:

```text
Push to main
      ↓
     CI
      ↓
   Build
      ↓
  Artifact
      ↓
   Deploy
      ↓
GitHub Pages
```

---

# 🏗️ Project Structure

```text
cici_c3/
│
├── .github/
│   └── workflows/
│       ├── main.yml
│       └── main1.yml
│
├── app.py
├── test_app.py
└── README.md
```

---

# 📂 File Explanation

## `app.py`

Contains a simple Python function used for demonstrating automated testing.

```python
def add(a, b):
    return a + b
```

---

## `test_app.py`

Contains a Pytest test that verifies the function.

```python
def test_add():
    assert add(2, 3) == 5
```

---

## `.github/workflows/main.yml`

This workflow demonstrates **Continuous Integration**.

It:

1. Runs when code is pushed
2. Creates an Ubuntu runner
3. Checks out the repository
4. Installs Python 3.12
5. Installs Pytest
6. Runs the tests

Pipeline:

```text
Push
 ↓
Checkout
 ↓
Setup Python
 ↓
Install Pytest
 ↓
Run Tests
 ↓
PASS / FAIL
```

---

## `.github/workflows/main1.yml`

This workflow demonstrates a complete **CI/CD pipeline** for the website.

It contains three stages:

```text
CI → BUILD → DEPLOY
```
