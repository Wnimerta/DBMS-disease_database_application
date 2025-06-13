# 🤟 Disease Database Application

A modern, intuitive desktop application that allows users to explore diseases across medical specialties, search by symptoms, and access detailed disease data. Built with **Python Tkinter** and **MySQL**, this educational tool bridges healthcare and technology.

---

## 🌎 Overview

The Disease Database Application was developed as part of the DBMS course at **Sukkur IBA University**. It is designed for students, researchers, and junior healthcare professionals to access disease-related information categorized by specialties.

> **Key Features**:
>
> * Browse diseases by medical specialty
> * Search diseases by keyword or symptom
> * View detailed symptom and organ information
> * Simple, clean, and interactive GUI

---

## 📆 Project Info

* **Course**: Database Management Systems (DBMS)
* **Submitted By**:

  * Rabia Soomro (CMS: 133-22-0025)
  * Nimerta Wadhwani (CMS: 133-22-0009)
  * Waqar Abbas (CMS: 133-22-0039)
* **Supervisor**: Mrs. Zainab Umair
* **Submission Date**: May 2025

---

## 🚀 Objectives

* Design a relational database for medical disease information
* Create a GUI to display and interact with database content
* Enable specialty-based browsing and symptom-based searching
* Display detailed disease descriptions
* Ensure application robustness and user-friendliness

---

## 🔧 Tech Stack

| Component            | Technology                  |
| -------------------- | --------------------------- |
| Programming Language | Python 3.x                  |
| GUI Framework        | Tkinter                     |
| Database             | MySQL (via mysql-connector) |
| IDE                  | Jupyter Notebook            |

---

## 📂 Database Structure

### 🔍 Specialties Table

* **SpecialtyID** (Primary Key)
* **SpecialtyName** (e.g., Cardiology, Dermatology)

### 🔰 Specialty Tables (e.g., Pediatricians, Dermatologists)

* **DiseaseName**
* **Symptoms\_1**, **Symptoms\_2**, **Symptoms\_3**
* **AffectedOrgan\_1**, **AffectedOrgan\_2**
* **SpecialtyID** (Foreign Key)

> Total: 10 specialties x 10 diseases = 100 entries

---

## 💻 GUI Design

* **Dropdown Menu**: Select medical specialty
* **Search Bar**: Type keyword or symptom
* **Listbox**: Displays disease names with symptoms & affected organs
* **Details Section**: Shows full disease data on click
* **Theme**: Clean light blue (#e6f0fa)

---

## 🔢 How to Run

```bash
# Clone the repository
$ git clone https://github.com/your-username/disease-database-app.git
$ cd disease-database-app

# Install dependencies
$ pip install mysql-connector-python

# Configure your MySQL credentials in db_config

# Run the application
$ python disease_app.py
```

---

## 📊 Features in Action

* Select "Dermatology" to see 10 related diseases
* Search "fever" to get diseases from multiple specialties
* Click on "Acne" to see all its symptoms and organs

---

## 🚫 Challenges Solved

* ❌ **SpecialtyID Errors**: Removed redundant filters to fix query issues
* ❌ **Empty Results After Search**: Modified search to scan across all tables
* ❌ **MySQL Connection Issues**: Handled through correct configuration and error messages
* ❌ **GUI Crashes in Jupyter**: Optimized by modular cell execution and debug logs

---

## 👥 Team Contributions

| Team Member      | Role & Contribution                       |
| ---------------- | ----------------------------------------- |
| Rabia Soomro     | Designed & populated MySQL database       |
| Nimerta Wadhwani | Developed GUI layout and styling          |
| Waqar Abbas      | Coded core logic, search & detail methods |

---

## 🚀 Future Enhancements

* Add more diseases and specialties
* Advanced search filters (e.g., by affected organ)
* GUI enhancements and visual themes
* Convert to standalone `.exe` using PyInstaller

---

## 📖 References

* [MySQL Docs](https://dev.mysql.com/doc/refman/8.0/en/)
* [Tkinter Documentation](https://docs.python.org/3/library/tkinter.html)
* [W3Schools SQL](https://www.w3schools.com/sql/)
* [TutorialsPoint Python GUI](https://www.tutorialspoint.com/python/python_gui_programming.htm)

---

> ✨ *An educational desktop tool bridging computer systems and healthcare.*
