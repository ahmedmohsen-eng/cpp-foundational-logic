# C++ Foundational Logic & Mathematical Implementations

This repository serves as a professional portfolio of low-level software implementations. The primary objective is to demonstrate the translation of mathematical theorems and logical principles into robust, production-ready C++ code without relying on high-level external libraries.

---

## 🚀 Projects Overview

### 1. Chronological Logic: Day-of-the-Week Calculator

A manual implementation of chronological arithmetic to determine the day of the week for any date after the year 1600.

**Engineering Focus**
- Avoids `<chrono>` and other high-level utilities.
- Implements anchor-day logic manually.
- Performs leap-year calculation using:

```cpp
year % 400 == 0 || (year % 4 == 0 && year % 100 != 0)
```

**Logic**
- Uses modular arithmetic to align day offsets within a 7-day cycle.

---

### 2. Cryptographic Foundations: Caesar Cipher

A hardened implementation of the classic Caesar Cipher for encryption and decryption.

**Engineering Focus**
- Character-set transformations
- Supports both positive and negative key shifts
- Ensures mathematical consistency

**Mathematical Rule**

```
E(x) = (x + k) mod 26
```

---

## 🛠 Engineering Excellence & Robustness

A defining feature of these implementations is **Input Stream Hardening**, ensuring resilience against malformed or invalid user input.

### Failure Resilience
- Uses:
  - `std::numeric_limits<streamsize>::max()`
  - `cin.clear()`
- Prevents infinite loops caused by incorrect data types.

### Edge-Case Validation
- Rejects non-numeric keys where integers are required.
- Rejects invalid dates (e.g., year < 1601).
- Rejects mixed strings such as `"123abcd"` when numeric input is expected.

### Zero-Dependency Design
Every algorithm is built from first principles to demonstrate a deep understanding of:
- Logical reasoning
- Mathematical translation
- Low-level system behavior

---

## 📂 Repository Structure

```
├── caesar-cipher/
│   └── main.cpp        # Cipher logic with input hardening
├── day-of-week/
│   └── main.cpp        # Chronological logic and leap-year math
└── README.md           # Project documentation
```

---

## 💻 How to Run

Ensure you have a C++ compiler installed (GCC or Clang).

### Clone the repository

```bash
git clone https://github.com/ahmedmohsen-eng/cpp-foundational-logic.git
```

### Navigate to the desired project directory and compile

```bash
g++ main.cpp -o program
```

### Run the executable

```bash
./program
```

---

## 👨‍💻 Author

**Ahmed Mohsen**  
**Focus:** Computer Engineering | Algorithms | System-Level Problem Solving
