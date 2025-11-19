# 🚌 BUS BOOKING WEB APPLICATION
*A Complete Online Bus Ticket Booking System — Flask + MySQL + AWS EC2*

Welcome to the **Bus Booking App**, a lightweight and production-ready web application that lets users search buses, select routes, book seats, and download tickets — all through a simple, clean interface.

---

## 📌 1. Overview

This is an end-to-end **Flask** project connected with **MySQL** and deployable on **AWS EC2**.  
The application provides:

- ✔️ View available buses  
- ✔️ Search route and journey date  
- ✔️ Book a seat  
- ✔️ Download ticket as a file  
- ✔️ Data stored in MySQL  
- ✔️ Fast, clean & user-friendly UI

---

## ⚙️ 2. Technologies Used

| Category      | Technology        |
|---------------|-------------------|
| 🟦 Language   | Python 3          |
| 🧪 Framework  | Flask             |
| 🎨 Frontend   | HTML, CSS         |
| 🗄️ Database   | MySQL             |
| ☁️ Cloud      | AWS EC2           |
| 🧰 Versioning | Git & GitHub      |

---

## 🧱 3. Project Structure
```

bus_booking_app/
├── app.py
├── database/
│ └── schema.sql
├── requirements.txt
├── static/
│ └── style.css
└── templates/
├── index.html
├── book.html
├── success.html
└── ticket.html
```


## 🚀 4. Features

- 🔍 Search and view available buses  
- 🗺️ Route selection and journey date filters  
- 🙍 Passenger information form and seat selection  
- 🎟️ Instant booking confirmation  
- ⬇️ Download ticket as HTML (use a converter to PDF if needed)  
- 💾 Persistent storage in MySQL  
- ⚡ Responsive and lightweight UI

---

## 📥 5. Installation & Setup

### 🔧 Step 1 — Install Dependencies
```
pip install -r requirements.txt
```
### 🗄️ Step 2 — Setup the Database
```
mysql -u root -p < database/schema.sql
```
### ▶️ Step 3 — Run the Application (development)
```
python3 app.py
🌐 Open in Browser
Visit: http://127.0.0.1:5000/
```
### 🧠 6. How It Works
```
User visits homepage and sees available buses.

User selects route + journey date and clicks Book.

User fills passenger details and confirms booking.

System saves booking to MySQL and shows success page.

User can download/open the ticket page (save as PDF if needed).
```
### 📸 7. Recommended Screenshots

Place screenshots in /screenshots folder and link them like this:

🚌 Available Buses

📝 Booking Page

🎟️ Ticket Download

If you prefer direct image links (already hosted), replace the screenshots/... path with your hosted URL.

-----
### 📦 8. Database:
```
Create a simple database/schema.sql like:

CREATE DATABASE IF NOT EXISTS bus_booking;
USE bus_booking;

CREATE TABLE buses (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(255),
  route_from VARCHAR(255),
  route_to VARCHAR(255),
  departure_time TIME,
  arrival_time TIME,
  price DECIMAL(8,2),
  seats_total INT
);

CREATE TABLE bookings (
  id INT AUTO_INCREMENT PRIMARY KEY,
  bus_id INT,
  passenger_name VARCHAR(255),
  passenger_email VARCHAR(255),
  seat_number VARCHAR(20),
  journey_date DATE,
  booked_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  FOREIGN KEY (bus_id) REFERENCES buses(id)
);
```
----
### ⚙️ 9. Deployment (quick tip)
For production on AWS EC2:

Use Gunicorn + Nginx (Gunicorn serves Flask, Nginx as reverse proxy).

Secure MySQL (use RDS or secure EC2-hosted MySQL).

Use environment variables for DB credentials.

Configure firewall (security group) to allow only required ports (80/443).
If you want, I can provide a full deploy.md with exact commands.

### 📬 10. Author
Prasad
Cloud & DevOps Engineer — building simple, scalable apps.
----
### ⭐ 11. Contribution & Support
If you like this project:

⭐ Star the repo

🍴 Fork it

🐛 Open issues or contribute PRs

----
### 🔒 12. Notes
This README is optimized for clarity and copying to README.md.

Replace placeholder screenshots and database credentials with your real data before publishing.

Made with ❤️ by Prasad

----
## 📩 Connect With Me

If you’d like to collaborate, discuss projects, or just say hello — feel free to reach out!

### 🔗 **Social & Professional Links**

- 🌐 [Portfolio Website](https://prasad-bhoite19.github.io/prasad-portfolio/)  
- 💼 [LinkedIn](http://linkedin.com/in/prasad-bhoite-a38a64223)  
- 🐙 [GitHub](https://github.com/Prasad-bhoite19) 
- ✉️ [Email](prasadsb2002@gmail.com)   


💬 Always open for opportunities in **Cloud, DevOps, and Full-Stack Projects**.



