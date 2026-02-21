C++ Foundational Logic & Mathematical Implementations

This repository serves as a professional portfolio of low-level software implementations. The primary objective is to demonstrate the translation of mathematical theorems and logical principles into robust, production-ready C++ code without relying on high-level external libraries.

🚀 Projects Overview

1. Chronological Logic: Day-of-the-Week Calculator

A manual implementation of chronological arithmetic to determine the day of the week for any date after the year 1600.

Engineering Focus: Instead of using <chrono>, this implementation utilizes anchor-day logic and manual leap-year calculations (year % 400 == 0 || (year % 4 == 0 && year % 100 != 0)).

Logic: Handles modular arithmetic to align day-offsets within a 7-day week cycle.

2. Cryptographic Foundations: Caesar Cipher

A hardened implementation of the classic Caesar Cipher for text encryption and decryption.

Engineering Focus: Focuses on character-set transformations and mathematical consistency for both positive and negative key shifts.

Mathematical Rule: Implemented using the formula: E(x) = (x + k) mod 26.

🛠 Engineering Excellence & Robustness

A key feature of these implementations is the emphasis on Input Stream Hardening. Unlike basic student scripts, this code is designed to handle malformed user input gracefully:

Failure Resilience: Uses std::numeric_limits<streamsize>::max() and cin.clear() to sanitize input buffers and prevent infinite loops on invalid data types.

Edge-Case Validation: * Rejects non-numeric keys where integers are expected.

Validates year constraints (e.g., rejecting dates before 1601 for the chronological algorithm).

Handles mixed input strings (e.g., rejecting "123abcd" when a pure number is required).

Zero-Dependency Design: Every algorithm is built from first principles to demonstrate a deep understanding of the underlying logic and system behavior.

📂 Repository Structure

├── caesar-cipher/
│   └── main.cpp        # Cipher logic with input hardening
├── day-of-week/
│   └── main.cpp        # Chronological logic and leap-year math
└── README.md           # Project documentation



💻 How to Run

Ensure you have a C++ compiler installed (GCC/Clang).

Clone the repository:

git clone [https://github.com/ahmedmohsen-eng/cpp-foundational-logic.git](https://github.com/ahmedmohsen-eng/cpp-foundational-logic.git)



Navigate to the desired project directory and compile:

g++ main.cpp -o program



Run the executable:

./program



Author: Ahmed Mohsen

Focus: Computer Engineering | Algorithms | System-Level Problem Solving
