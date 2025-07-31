# 🔐 Secure Password Generator with Entropy Checker

A Python-based secure password generator that uses the `secrets` module to create cryptographically strong passwords. It also calculates the **entropy** (i.e., the bits of randomness/security) of the generated password to give you a clear idea of its strength.

---

## 📂 File Structure

```
secure-password-generator/
├── password_generator.py   # Main script
└── README.md               # Documentation
```

---

## 🚀 Features

- ✅ Cryptographically secure password generation using `secrets`
- 🔣 Includes lowercase, uppercase, digits, and special characters
- 🔐 Calculates password entropy (strength in bits)
- 🔁 Option to regenerate until satisfied
- 🧠 Simple and interactive command-line interface

---

## 🛠️ Requirements

- Python 3.6+

No third-party packages required. Uses only Python’s standard library (`secrets`, `string`, `math`).

---

## ▶️ How to Run

1. Clone or download the project.
2. Open a terminal in the project directory.
3. Run the script:

```bash
python password_generator.py
```

---

## ✨ Example Usage

```
===== Secure Password Generator =====
Enter desired password length: 16

Generated Password: *T4bQ?Z9pd=KwI#m
Password Entropy: 104.00 bits
🔒 Strong password! Very secure.
Are you happy with this password? (yes/no): yes
✅ Password finalized.
```

---

## 🔐 Entropy Guide

| Entropy Bits | Strength         | Recommendation                        |
|--------------|------------------|----------------------------------------|
| < 50         | ⚠️ Weak          | Too easy to guess — increase length    |
| 50–80        | ✅ Moderate       | Acceptable but could be stronger       |
| > 80         | 🔒 Strong         | Highly secure                          |

---

## 📚 How It Works

- `generate_password(length)`  
  Creates a random password of specified length using all character types.

- `calculate_entropy(password)`  
  Estimates how unpredictable the password is, using:  
  `entropy = log2(pool_size^length)`

- Prompts user to accept or regenerate until satisfied.

---

## 📄 License

This project is open-source and free for personal or educational use.

---

