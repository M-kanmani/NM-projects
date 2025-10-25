Email Reminder System

A simple **Email Reminder Web Application** built with **HTML**, **CSS**, and **JavaScript**.  
It allows users to schedule and send email reminders at a specific date and time using **EmailJS**, without needing any backend server.

Features

Schedule reminder emails  
Custom message and time selection  
Sends emails using [EmailJS](https://www.emailjs.com/)  
Simple, clean, and responsive UI  
100% client-side — no backend needed  

Tech Stack

| Technology | Purpose |
|-------------|----------|
| **HTML5** | Page structure |
| **CSS3** | Styling and layout |
| **JavaScript (ES6)** | Logic, scheduling, and email sending |
| **EmailJS** | Send emails from client-side |

Folder Structure

email-reminder/
│
├── index.html # Main HTML file
├── style.css # Styling for the webpage
└── script.js # App logic and EmailJS integration

Setup Instructions

Clone the Repository
bash
git clone https://github.com/<your-username>/email-reminder-system.git
cd email-reminder-system
Set Up EmailJS
Go to EmailJS and create a free account.

Create a new Email Service (e.g., Gmail, Outlook).

Create an Email Template with variables:

css
To: {{to_email}}
Message: {{message}}
Copy the following from your EmailJS dashboard:

Service ID

Template ID

Public Key
Configure Your Credentials
In script.js, replace the placeholders with your real EmailJS credentials:

js
emailjs.init("YOUR_PUBLIC_KEY");
emailjs.send("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", templateParams);
 How to Run
Open index.html in your browser.

Enter:

Recipient Email

Message

Reminder Date & Time

Click Set Reminder.

The app waits until the selected time and automatically sends the reminder email.

How It Works
The user sets a reminder (email, message, time).

JavaScript calculates the delay (setTimeout) until the selected time.

When the time is reached, EmailJS sends the email using your configured template.


Future Enhancements
Add countdown timer for next reminder

Save reminders using Local Storage

Add notification sounds

Upgrade to backend-based system (Node.js + MongoDB)

Contributing
Contributions are always welcome!

Fork this repo

Create a new branch: git checkout -b feature/YourFeature

Commit your changes: git commit -m "Add new feature"

Push the branch: git push origin feature/YourFeature

Open a Pull Request

License
This project is licensed under the MIT License — you are free to use, modify, and distribute 

---
