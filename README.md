# Student Enrollment Form using JsonPowerDB

A responsive web-based **Student Enrollment System** built using **HTML, Bootstrap, JavaScript, AJAX, and JsonPowerDB (JPDB)**. The application enables users to add, update, reset, and manage student records efficiently using a simple user interface and a NoSQL database.

---

## 📌 Project Overview

This project demonstrates how to integrate a frontend web application with **JsonPowerDB (JPDB)** to perform CRUD (Create, Read, Update, Delete) operations. It provides an easy-to-use student enrollment form where users can enter student details and store them directly in the database.

The project is lightweight, beginner-friendly, and ideal for learning AJAX requests and JPDB integration.

---

## ✨ Features

* Add new student records
* Update existing student information
* Search student records using Roll Number
* Reset form fields
* Responsive user interface using Bootstrap
* Client-side validation
* Fast database operations using JsonPowerDB
* AJAX-based communication without page reload
* Simple and clean design

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* Bootstrap 5
* JavaScript (ES6)
* AJAX

### Database

* JsonPowerDB (JPDB)

---

## 📂 Project Structure

```text
student-enrollment-jsonpowerdb/
│
├── index.html          # Main webpage
├── style.css           # Custom styling (if used)
├── script.js           # JavaScript logic
├── README.md           # Project documentation
└── assets/             # Images or additional resources (optional)
```

---

## 📋 Student Information Collected

The enrollment form stores details such as:

* Roll Number
* Full Name
* Class
* Birth Date
* Address
* Enrollment Date

---

## ⚙️ How It Works

1. Open the Student Enrollment Form.
2. Enter the student's Roll Number.
3. If the Roll Number already exists:

   * Existing data is fetched from JsonPowerDB.
   * User can update the record.
4. If the Roll Number is new:

   * Fill in the remaining details.
   * Save the record into the database.
5. Use the Reset button to clear all fields.

---

## 🚀 Getting Started

### Prerequisites

* Web Browser
* Internet Connection
* JsonPowerDB Account
* JPDB Connection Token

### Installation

1. Clone the repository

```bash
git clone https://github.com/your-username/student-enrollment-jsonpowerdb.git
```

2. Navigate to the project folder

```bash
cd student-enrollment-jsonpowerdb
```

3. Open `index.html` in your browser.

---

## 🔗 JsonPowerDB Configuration

Before running the project, configure the following values inside your JavaScript file:

* Database Name
* Relation Name
* Connection Token
* JPDB API URL

Example:

```javascript
const connToken = "YOUR_CONNECTION_TOKEN";
const dbName = "YOUR_DATABASE_NAME";
const relName = "STUDENT-TABLE";
```

Replace these values with your own JsonPowerDB credentials.

---

## 💡 Advantages of JsonPowerDB

* High-performance NoSQL database
* Simple REST API
* Schema-free architecture
* Lightweight and fast
* Easy integration with JavaScript
* Low development effort
* Real-time data operations

---

## 📸 Screenshots

You can include screenshots like:

* Home Page
* Student Enrollment Form
* Successfully Saved Record
* Update Record
* Database Records

Example:

```text
screenshots/
├── home.png
├── save.png
├── update.png
└── database.png
```

---

## 🎯 Future Enhancements

* Delete student records
* Search by multiple fields
* Student list dashboard
* Pagination
* Authentication and Login
* Export records to Excel or PDF
* Improved form validation
* Responsive dashboard with charts

---

## 📖 Learning Outcomes

Through this project, you will learn:

* HTML form design
* Bootstrap responsive layouts
* JavaScript DOM manipulation
* AJAX requests
* REST API integration
* CRUD operations
* JsonPowerDB usage
* Client-side validation

---

## 🤝 Contributing

Contributions are welcome!

If you'd like to improve this project:

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License.

---

## 👩‍💻 Author

**Anisha Garg**

* B.Tech CSE (AI & ML)
* VIT Bhopal University

GitHub: https://github.com/Ani-sha23

---

## ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub. It helps others discover the project and motivates future improvements.
