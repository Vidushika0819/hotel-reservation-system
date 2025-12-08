# Hotel Reservation System

**A web-based Hotel Reservation Management System built with PHP and MySQL.**  
This project includes user reservation booking, admin management, venue handling, payment simulation, and full CRUD operations for users, venues, and reservations.

---

## 🔧 Features
- User registration and login  
- Search and book hotel venues/rooms  
- Admin dashboard to manage users, venues and reservations (CRUD)  
- User dashboard to view and cancel reservations  
- Simulated payment page (fake_payment.php)  
- File upload support for venue images  
- SQL script to create database and tables

---

## 🛠 Tech stack
- Backend: PHP  
- Frontend: HTML, CSS (inside PHP pages)  
- Database: MySQL (SQL dump included)  
- Development server: XAMPP / WAMP / LAMP

---

## 🚀 Quick setup (Local development)

1. Install XAMPP or WAMP (for Windows) or LAMP (Linux).  
2. Copy the project folder into your web server folder:
   - XAMPP: `C:\xampp\htdocs\hotel-reservation-system`
3. Create a MySQL database:
   - Open phpMyAdmin → Create database: `hotel_reservation_db`
4. Import SQL:
   - In phpMyAdmin select `hotel_reservation_db` → Import → choose `database/hotel_reservation.sql`
   - OR run: `mysql -u root -p hotel_reservation_db < hotel_reservation.sql`
5. Configure database connection:
   - Open the file that contains DB connection settings (commonly named `db_connect.php`, `config.php`, or similar) inside `src/` and update host, username, password, database name.
     ```php
     // example
     $conn = new mysqli('localhost','root','','hotel_reservation_db');
     ```
6. Start Apache and MySQL in XAMPP.  
7. Open browser → `http://localhost/hotel-reservation-system/src/index.php`

---

## 📁 Project structure
```
hotel-reservation-system/
├─ src/ # PHP pages and server logic (user, admin pages)
├─ assets/
│ ├─ images/ # venue/user images
│ └─ uploads/
├─ database/
│ └─ hotel_reservation.sql
└─ README.md
```
---

## ✅ Notes & tips
- For security, do not commit files that contain real credentials. Use environment variables or a config file that you exclude via `.gitignore`.
- Consider sanitizing user inputs before DB queries to prevent SQL injection (use prepared statements).
- Add instructions for admin credentials in the README if you want reviewers to test admin features.

---

## 📞 Contact
Vidushika Madhushani — Vidushika0819 on GitHub  
Email: [withanagevidhu@gmail.com]

---

## 📄 License
This project is released under the MIT License. See `LICENSE`.
