
# Student Enrollment Form using JsonPowerDB

<p align="center">
  <img src="https://img.shields.io/badge/Project-Student%20Enrollment-6366F1?style=for-the-badge&logo=googleclassroom&logoColor=white" alt="Project Badge" />
  <img src="https://img.shields.io/badge/Database-JsonPowerDB-0EA5E9?style=for-the-badge" alt="Database Badge" />
  <img src="https://img.shields.io/badge/Frontend-HTML%20%7C%20Bootstrap%20%7C%20JavaScript-F59E0B?style=for-the-badge" alt="Frontend Badge" />
</p>

<p align="center">
  A simple, responsive, and efficient web application for managing student enrollment records using <b>JsonPowerDB (JPDB)</b>.
</p>

<p align="center">
  <b>Enroll Students &nbsp; | &nbsp; Search Records &nbsp; | &nbsp; Update Details</b>
</p>

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Student Information](#student-information)
- [Getting Started](#getting-started)
- [JsonPowerDB Configuration](#jsonpowerdb-configuration)
- [Application Workflow](#application-workflow)
- [Why JsonPowerDB?](#why-jsonpowerdb)
- [Screenshots](#screenshots)
- [Future Enhancements](#future-enhancements)
- [Learning Outcomes](#learning-outcomes)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

---

## Overview

**Student Enrollment Form using JsonPowerDB** is a responsive web application designed to simplify the process of collecting and managing student information.

Built with **HTML5, Bootstrap, JavaScript, AJAX, and JsonPowerDB**, the application demonstrates how a frontend interface can communicate with a NoSQL database to perform student record operations without reloading the page.

The project focuses on simplicity, efficient data handling, user-friendly form interactions, and practical database integration.

### Project Objectives

- Build a clean and responsive student enrollment interface.
- Integrate a web application with JsonPowerDB.
- Perform Create, Read, and Update operations on student records.
- Validate student information before submission.
- Understand AJAX-based communication with database APIs.

---

## Features

| Feature | Description |
|---|---|
| Add Student | Register new student records in the database. |
| Search Student | Retrieve student information using Roll Number. |
| Update Record | Modify existing student information. |
| Reset Form | Clear input fields and prepare the form for another entry. |
| Responsive UI | Use a Bootstrap-based interface across screen sizes. |
| Form Validation | Validate required fields before processing data. |
| AJAX Integration | Communicate with the database without a full-page reload. |
| Database Integration | Store and retrieve records through JsonPowerDB. |
| Simple Interface | Keep enrollment operations straightforward and accessible. |

> **Note:** The available operations depend on the functionality implemented in the application. Delete functionality is listed as a future enhancement.

---

## Tech Stack

<p>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white" alt="Bootstrap" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/AJAX-0078D4?style=flat-square" alt="AJAX" />
  <img src="https://img.shields.io/badge/JsonPowerDB-NoSQL-0EA5E9?style=flat-square" alt="JsonPowerDB" />
</p>

| Technology | Purpose |
|---|---|
| HTML5 | Structures the enrollment form. |
| CSS3 | Provides custom styling when required. |
| Bootstrap 5 | Creates responsive layouts and UI components. |
| JavaScript (ES6) | Handles form logic, validation, and interactions. |
| AJAX | Sends asynchronous database requests. |
| JsonPowerDB (JPDB) | Stores and retrieves student records. |

---

## Project Structure

```text
student-enrollment-jsonpowerdb/
│
├── index.html          # Main enrollment webpage
├── style.css           # Custom CSS styling (if used)
├── script.js           # JavaScript and JPDB integration
├── README.md           # Project documentation
│
└── assets/             # Images and additional resources (optional)
    └── screenshots/    # Application screenshots (optional)
```

*The actual folder and file names may differ depending on your implementation.*

---

## Student Information

The application is designed to collect and manage the following student details:

| Field | Description |
|---|---|
| Roll Number | Unique student identifier |
| Full Name | Student's name |
| Class | Student's class or section |
| Birth Date | Student's date of birth |
| Address | Student's residential address |
| Enrollment Date | Date of enrollment |

The Roll Number is used to identify and retrieve existing student records.

---

## Getting Started

Follow these steps to set up the project locally.

### 1. Prerequisites

Make sure you have:

- A modern web browser.
- Git installed on your computer.
- A JsonPowerDB account and access to its API.
- The required database configuration and connection token.
- A code editor such as Visual Studio Code.

### 2. Clone the Repository

Replace the repository URL below with your actual GitHub repository URL.

```bash
git clone https://github.com/YOUR_USERNAME/student-enrollment-jsonpowerdb.git
```

### 3. Navigate to the Project Folder

```bash
cd student-enrollment-jsonpowerdb
```

### 4. Configure the Database

Open your JavaScript file and configure the required JsonPowerDB connection details according to the API integration used in your project.

### 5. Run the Application

Open `index.html` in your browser, or use the **Live Server** extension in Visual Studio Code.

> **Important:** Opening the page only runs the frontend. Database operations require a valid JsonPowerDB configuration, network access, and any necessary API permissions.

---

## JsonPowerDB Configuration

JsonPowerDB is used as the database layer for storing and retrieving student records.

Configure the following values in your JavaScript file, adapting the variable names to match your implementation:

```javascript
const connToken = "YOUR_CONNECTION_TOKEN";
const dbName = "YOUR_DATABASE_NAME";
const relName = "STUDENT-TABLE";
```

Also verify the following:

- **Connection Token:** Use the correct token for your database connection.
- **Database Name:** Specify the database created for the project.
- **Relation Name:** Specify the relation or table used for student records.
- **API Endpoint:** Use the appropriate endpoint for your JPDB API version.
- **Record Identifier:** Use Roll Number consistently when retrieving or updating records.

### Security Best Practices

- Never commit real connection tokens, passwords, or private credentials to a public repository.
- Avoid exposing sensitive credentials in client-side JavaScript.
- Use a secure backend proxy for sensitive operations when appropriate.
- Restrict database permissions and rotate exposed credentials.
- Store configuration secrets in environment variables on the server side where applicable.

**Important:** Client-side environment variables are not secret once included in publicly served JavaScript. A private token should not be placed in a public frontend repository.

---

## Application Workflow

```text
        ┌─────────────────────────┐
        │   Open Enrollment Form  │
        └────────────┬────────────┘
                     │
                     ▼
        ┌─────────────────────────┐
        │ Enter Student Roll No.  │
        └────────────┬────────────┘
                     │
                     ▼
        ┌─────────────────────────┐
        │ Search JsonPowerDB      │
        └────────────┬────────────┘
                     │
              ┌──────┴──────┐
              ▼             ▼
       Record Exists    New Record
              │             │
              ▼             ▼
       Load Existing    Enter Student
          Details         Details
              │             │
              ▼             ▼
        Update Record    Save Record
              │             │
              └──────┬──────┘
                     ▼
        ┌─────────────────────────┐
        │ Display Operation Result│
        └─────────────────────────┘
```

### How It Works

1. Open the student enrollment form.
2. Enter a student's Roll Number.
3. Search the database for the specified Roll Number.
4. If the record exists, retrieve its details and allow the user to update them.
5. If the record is new, enter the remaining information and save it.
6. Use the Reset button to clear the form when needed.

---

## Why JsonPowerDB?

JsonPowerDB offers a lightweight database integration approach for small web applications and learning projects.

- **Fast Integration:** Work with database operations through APIs.
- **Schema Flexibility:** Work with JSON-based data structures.
- **REST API Support:** Connect frontend or backend applications to database services.
- **Lightweight Workflow:** Reduce setup complexity for suitable projects.
- **Learning Friendly:** Practice database operations and API integration.

---

## Screenshots

Add screenshots of your actual application to showcase its interface and functionality.

Suggested folder structure:

```text
assets/
└── screenshots/
    ├── home.png
    ├── enrollment-form.png
    ├── saved-record.png
    ├── update-record.png
    └── database-records.png
```

Once you add the screenshots, display them in this section using the following Markdown:

### Home Page

![Student Enrollment Home Page](assets/screenshots/home.png)

### Enrollment Form

![Student Enrollment Form](assets/screenshots/enrollment-form.png)

### Saved Student Record

![Saved Student Record](assets/screenshots/saved-record.png)

### Updated Student Record

![Updated Student Record](assets/screenshots/update-record.png)

> Replace these example image paths with the actual screenshot filenames in your repository. Remove any image entries for screenshots you have not added yet.

---

## Future Enhancements

The following improvements could extend the application:

- [ ] Delete student records.
- [ ] Add advanced search and filtering.
- [ ] Create a student records dashboard.
- [ ] Add pagination for large datasets.
- [ ] Implement authentication and role-based access.
- [ ] Export student data to Excel or PDF.
- [ ] Improve input validation and error handling.
- [ ] Add success and error notifications.
- [ ] Introduce analytics and visual reports.
- [ ] Improve accessibility and responsive design.
- [ ] Add automated tests for form and database operations.

---

## Learning Outcomes

This project provides practical experience with:

- HTML form design and semantic markup.
- Responsive UI development with Bootstrap.
- JavaScript DOM manipulation and event handling.
- Client-side form validation.
- AJAX requests and asynchronous programming.
- REST API integration.
- Create, Read, and Update database operations.
- JSON-based data exchange.
- NoSQL database concepts.
- Git and GitHub project documentation.

---

## Contributing

Contributions, suggestions, and improvements are welcome!

To contribute:

1. Fork this repository.
2. Create a feature branch.

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. Commit your changes.

   ```bash
   git commit -m "Add your feature"
   ```

4. Push the branch.

   ```bash
   git push origin feature/your-feature-name
   ```

5. Open a Pull Request describing your changes.

---

## License

This project is intended to be released under the **MIT License**.

If you choose the MIT License, add a `LICENSE` file containing the appropriate license text to your repository.

---

## Author

### Anisha Garg

**B.Tech Computer Science Engineering — Artificial Intelligence & Machine Learning**

<p>
  <a href="https://github.com/Ani-sha23">
    <img src="https://img.shields.io/badge/GitHub-Ani--sha23-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Profile" />
  </a>
</p>

**GitHub Profile:** [github.com/Ani-sha23](https://github.com/Ani-sha23)

---

<p align="center">
  <b>If you find this project useful, consider giving the repository a star!</b>
</p>

<p align="center">
  Built using HTML, Bootstrap, JavaScript, AJAX, and JsonPowerDB.
</p>
