# 📧 XKCD Comic Mailer

**XKCD Comic Mailer** is a PHP-based subscription service that sends a random XKCD comic to registered users every day. It includes a two-step email verification process for both subscribing and unsubscribing, with all subscriber data stored in a flat file.

---

## ✨ Features

- **Email Registration**: Secure user registration with a 6-digit email verification code.
- **Daily XKCD Comics**: A CRON job automatically fetches a random XKCD comic and emails it to all subscribers every 24 hours.
- **Unsubscribe Mechanism**: Users can easily unsubscribe through a verified, two-step process.
- **File-Based Storage**: Uses a simple `.txt` file for storing subscriber emails, requiring no database setup.

---

## 🛠️ Tech Stack & Prerequisites

- PHP 8.3+
- A web server (e.g., Apache, Nginx)
- A server environment with CRON task scheduling enabled
- A configured Mail Transfer Agent (MTA) for PHP's `mail()` function to work

---

## 🚀 Getting Started

### 1. Installation

Clone the repository to your local machine or server:

```bash
git clone https://github.com/Harshithappu-2003/php-xkcd-mailer.git
cd php-xkcd-mailer

### 📝 How to Use
## Subscribing
Open index.php in your browser.

Enter your email address and submit the form.

Check your inbox for a 6-digit verification code.

Enter the code on the page to confirm your subscription.

## Unsubscribing
Click the "Unsubscribe" link in any comic email you receive.

You will be taken to unsubscribe.php.

Enter your email address to receive an unsubscription code.

Enter the code on the page to be removed from the list.

### 📁 File Structure
php-xkcd-mailer/
│
├── index.php               # Main landing and registration page
├── unsubscribe.php         # Handles user unsubscription
└── src/
    ├── functions.php       # Core application logic
    ├── cron.php            # Script executed by the CRON job
    ├── setup_cron.sh       # Script to configure the CRON job
    └── registered_emails.txt # Flat file used to store subscriber emails

![1](https://github.com/user-attachments/assets/a0ed33d3-6871-46f4-afc9-683924985fa5)
![2](https://github.com/user-attachments/assets/377c0007-dad4-4fbc-886a-9ea4e1fd18c8)
![3](https://github.com/user-attachments/assets/f89867d8-554d-4974-90ee-a61e8ffbed93)
![4](https://github.com/user-attachments/assets/531e703e-9f3d-40cc-b5b7-05234a533833)
![5](https://github.com/user-attachments/assets/55b66da8-ffe4-4a79-b027-ef560b2cd7ba)
![6](https://github.com/user-attachments/assets/2eb9d5c7-bef2-4e89-ba83-3bec8bb322d9)
![7](https://github.com/user-attachments/assets/ecbc8202-0d43-45cc-a1e3-17002970c6d4)
![8](https://github.com/user-attachments/assets/2cc6f4f9-3f23-4f63-8198-273dd1fbe670)




