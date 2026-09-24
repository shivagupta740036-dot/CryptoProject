# 🔐 Ancient Encoder

### Ancient Wisdom. Digital Encoding.

Ancient Encoder is an educational web application that connects **ancient Indian knowledge systems** with **modern digital encoding concepts**.

The project demonstrates how traditional number-based knowledge systems can be explored alongside modern techniques such as **ASCII, Binary, and Caesar Cipher** through an interactive and beginner-friendly interface.

---

## ✨ Features

* 🏠 Modern and responsive home page
* 🔐 Multiple encoding methods
* 🇮🇳 Katapayadi encoding
* 🕉️ Bhuta Sankhya encoding
* 🔤 ASCII encoding and decoding
* 💻 Binary encoding and decoding
* 🔄 Caesar Cipher with shift control
* 📋 Copy encoded/decoded results
* 🔁 Swap input and output
* 🧹 Clear workspace
* 📥 Download generated output
* 👤 User registration and login
* 📊 User dashboard
* 📝 Encoding history
* 🧠 Learning section
* 🎯 Practice/quiz section
* 🤖 AI learning assistant interface
* 📱 Responsive design for mobile, tablet and desktop
* 🎨 Indian heritage inspired light UI
* ✨ Smooth and subtle animations
* 💾 SQLite database support
* 🔒 Password hashing and session-based authentication

---

## 🛠️ Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript
* Tailwind CSS
* Lucide Icons

### Backend

* Python
* Flask
* REST API

### Database

* SQLite

### Security

* Flask Sessions
* Werkzeug Password Hashing

### Testing

* Python testing
* JavaScript validation
* API testing

---

## 📚 Encoding Methods

### 1. Caesar Cipher

A simple substitution cipher where each letter is shifted by a selected number.

Example:

```text
HELLO
Shift = 3

KHOOR
```

---

### 2. Katapayadi

Katapayadi is a traditional Indian system that associates Sanskrit consonants with numerical values.

Example:

```text
क → 1
ख → 2
ग → 3
घ → 4
```

The project uses an educational mapping to demonstrate the concept interactively.

---

### 3. Bhuta Sankhya

Bhuta Sankhya is a traditional Indian numerical system where familiar concepts or objects represent numbers.

Example:

```text
Moon → 1
Eyes → 2
Vedas → 4
Seasons → 6
Sky → 0
```

The implementation is designed for educational demonstration.

---

### 4. ASCII

ASCII represents characters using numerical values.

Example:

```text
A → 65
B → 66
C → 67
```

---

### 5. Binary

Binary represents data using only:

```text
0
1
```

Example:

```text
A → 01000001
```

---

## 🖥️ Project Structure

```text
Ancient-Encoder/
│
├── app.py
├── requirements.txt
├── README.md
├── LICENSE
├── .gitignore
├── .env.example
├── TEST_REPORT.md
├── CHANGELOG.md
│
├── templates/
│   └── index.html
│
├── static/
│   ├── css/
│   │   └── style.css
│   │
│   ├── js/
│   │   ├── app.js
│   │   ├── auth.js
│   │   ├── encoder.js
│   │   ├── dashboard.js
│   │   ├── quiz.js
│   │   └── ai.js
│   │
│   └── assets/
│
├── database/
│   └── README.md
│
└── tests/
    ├── test_app.py
    ├── test_encoders.py
    └── test_api.py
```

---

# 🚀 Installation

## 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Move into the project:

```bash
cd Ancient-Encoder
```

---

## 2. Create Virtual Environment

### Windows

```powershell
py -m venv venv
```

Activate it:

```powershell
.\venv\Scripts\Activate.ps1
```

---

## 3. Install Dependencies

```powershell
pip install -r requirements.txt
```

---

## 4. Run the Application

```powershell
py app.py
```

The application will normally run at:

```text
http://127.0.0.1:5000
```

Open the address in your browser.

---

# 🔐 Authentication

Users can create an account and log in.

The application stores:

* Username
* Hashed password
* Account creation date

Passwords are **not stored as plain text**.

---

# 💾 Database

SQLite is used for local data storage.

Main tables:

### Users

```text
users
├── id
├── username
├── password_hash
└── created_at
```

### History

```text
history
├── id
├── user_id
├── method
├── action
├── input_text
├── output_text
└── created_at
```

---

# 🔌 API

The backend provides REST API endpoints.

| Method | Endpoint        | Purpose                |
| ------ | --------------- | ---------------------- |
| GET    | `/`             | Open application       |
| POST   | `/api/register` | Create account         |
| POST   | `/api/login`    | Login                  |
| POST   | `/api/logout`   | Logout                 |
| GET    | `/api/me`       | Get current user       |
| POST   | `/api/encode`   | Encode/decode data     |
| GET    | `/api/history`  | Get user history       |
| DELETE | `/api/history`  | Clear history          |
| GET    | `/api/bhuta`    | Get Bhuta Sankhya data |

---

# 🎨 Design

The UI follows a **modern Indian heritage + technology** concept.

### Design principles

* Warm cream background
* Saffron/terracotta accents
* Deep maroon
* Indian green
* Antique gold
* Clean white cards
* Subtle heritage patterns
* Rounded modern components
* Simple navigation
* Responsive layout

The design is inspired by Indian heritage without making the website visually overcrowded.

---

# 📱 Responsive Design

Ancient Encoder is designed to work on:

* 💻 Desktop
* 💻 Laptop
* 📱 Mobile
* 📱 Tablet

The layout automatically adjusts according to screen size.

---

# 🧪 Testing

Before publishing, test:

```text
✓ Home page
✓ Navigation
✓ Login
✓ Registration
✓ Logout
✓ Caesar Encode
✓ Caesar Decode
✓ Katapayadi Encode
✓ Katapayadi Decode
✓ Bhuta Sankhya
✓ ASCII Encode
✓ ASCII Decode
✓ Binary Encode
✓ Binary Decode
✓ Copy button
✓ Swap button
✓ Clear button
✓ Download button
✓ History
✓ Dashboard
✓ Responsive layout
```

Run tests with:

```powershell
python -m pytest
```

---

# ⚠️ Educational Purpose

Ancient Encoder is primarily an **educational project**.

The Katapayadi and Bhuta Sankhya implementations are simplified demonstrations intended to help users understand the concept.

ASCII and Binary are **encoding techniques**, not encryption methods.

Caesar Cipher is a basic educational cipher and should not be considered secure modern cryptography.

---

# 🔮 Future Improvements

Possible future versions can include:

* 🤖 Real AI-powered learning assistant
* 🎤 Voice input
* 🔊 Text-to-speech
* 🌐 Multi-language support
* 📈 Advanced learning analytics
* 🏆 Gamification
* 🧩 More ancient Indian numerical systems
* 🔐 Modern cryptographic algorithms
* ☁️ Cloud database
* 👥 User profiles
* 📚 More educational content
* 📊 Advanced dashboard
* 📱 Progressive Web App support

---

# 👨‍💻 Author

**Shivam Gupta**

BSc IT Student

This project was created as an educational project combining:

```text
Ancient Indian Knowledge
        +
Computer Science
        +
Digital Encoding
        +
Web Development
```

---

# 📄 License

This project is intended for educational and learning purposes.

See the `LICENSE` file for license information.

---

## ⭐ Project Goal

> **Learn from the past. Build with technology.**

Ancient Encoder aims to make computer science concepts more interesting by presenting them through the connection between **ancient knowledge and modern technology**.
