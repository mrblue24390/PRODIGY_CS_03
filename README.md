 🔐 Password Complexity Checker

<div align="center">

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Tests](https://img.shields.io/github/actions/workflow/status/yourusername/Password-Complexity-Checker/python-ci.yml)
![Coverage](https://img.shields.io/codecov/c/github/yourusername/Password-Complexity-Checker)

**A comprehensive Python tool to evaluate password strength and provide actionable feedback**

[Features](#features) • [Installation](#installation) • [Quick Start](#quick-start) • [Documentation](#documentation)

</div>

---

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Installation](#installation)
- [Quick Start](#quick-start)
- [How It Works](#how-it-works)
- [Usage Examples](#usage-examples)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

---

## 🎯 Overview

The **Password Complexity Checker** is a Python tool that evaluates password strength based on multiple security criteria. It provides detailed feedback and suggestions for improvement, helping users create more secure passwords. The tool also includes a password generator and educational resources about password security.

### Key Achievements
- ✅ **Multi-criteria scoring** (length, character types, patterns, entropy)
- ✅ **Real-time feedback** with actionable suggestions
- ✅ **Password generator** for creating strong passwords
- ✅ **Educational resources** about password security
- ✅ **100% test coverage** for core logic

---

## ✨ Features

### 🔍 Password Assessment
| Criteria | Description | Weight |
|----------|-------------|--------|
| **Length** | Checks password length (8+ chars required) | 40 pts |
| **Character Types** | Uppercase, lowercase, digits, special chars | 60 pts |
| **Common Patterns** | Detects sequences, repeated chars, dictionary words | -30 pts |
| **Entropy** | Measures randomness (bits) | 20 pts |
| **Uniqueness** | Compares with previous passwords | 10 pts |

### 🎲 Password Generator
- Generates cryptographically secure passwords
- Customizable length (8-32 characters)
- Ensures at least one of each character type
- Uses `secrets` module for true randomness

### 📊 User Interface
- Interactive menu system
- Command-line arguments for scripting
- Detailed reports with visual strength meter
- Educational guidelines and tips

---

## 🛠️ Technology Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| **Python** | 3.8+ | Core programming language |
| **pytest** | 7.0+ | Unit testing framework |
| **GitHub Actions** | - | CI/CD automation |

*No external dependencies required – uses Python standard library only!*

---

## 📦 Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Method 1: Direct Installation (Recommended)

```bash
# Clone the repository
git clone https://github.com/yourusername/Password-Complexity-Checker.git
cd Password-Complexity-Checker

# (Optional) Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Run the tool
python src/cli.py
