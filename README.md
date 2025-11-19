# 🚌 Bus Booking App

A complete web-based **Bus Booking Application** that allows users to search, book, and manage bus tickets online.  
Built using **Python (Flask)**, **MySQL**, and deployed on **AWS EC2** .

🚀 Features

- 🔍 View available buses  
- 🗺️ Select route and journey details  
- 🎟️ Book a bus seat  
- ⬇️ Download booking ticket as a file  
- 💾 Data stored securely in MySQL database  
- ⚡ Fast and lightweight web application    

 🧱 Project Structure

 bus_booking_app
├── app.py
├── static
│   └── style.css
└── templates
    ├── book.html
    ├── index.html
    ├── success.html
    └── ticket.html

⚙️ Technologies Used

| Category | Technology |
|-----------|-------------|
| **Language** | Python 3 |
| **Framework** | Flask |
| **Frontend** | HTML, CSS |
| **Database** | MySQL |
| **Platform** | AWS EC2 (for hosting) |
| **Version Control** | Git & GitHub |

👉Install Dependencies
pip install -r requirements.txt

👉Setup the Databas
mysql -u root -p < database/schema.sql

👉Run the Application
python3 app.py

Then open your browser and visit:
👉 http://127.0.0.1:5000/

💡 How It Works

1.The user opens the app and sees a list of available buses.
2.The user selects the route and journey date.
3.The user enters booking details (name, seat, etc.).
4.After confirming, the user can download the ticket.
5.Simple, clean, and easy to use. 

📸 Screenshots

📸 Screenshots

👉Available Buses
<img width="1920" height="1080" alt="Screenshot 2025-10-04 123305" src="https://github.com/user-attachments/assets/6a75bf1d-5f19-4ae7-b62a-768c02b3af18" />

👉Booking Page
<img width="1920" height="1080" alt="Screenshot 2025-10-04 114438" src="https://github.com/user-attachments/assets/b53ede4d-51aa-4b80-8186-3e8e95492147" />

👉Ticket Download
<img width="1920" height="1080" alt="Screenshot 2025-10-04 123448" src="https://github.com/user-attachments/assets/cd6aac69-a6f8-46d1-a1d6-c47f6f439c31" />
