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

## 📝 How to Use
# Subscribing
- Open index.php in your browser.

- Enter your email address and submit the form.

- Check your inbox for a 6-digit verification code.

- Enter the code on the page to confirm your subscription.

# Unsubscribing
- Click the "Unsubscribe" link in any comic email you receive.

- You will be taken to unsubscribe.php.

- Enter your email address to receive an unsubscription code.

- Enter the code on the page to be removed from the list.

## 📁 File Structure

php-xkcd-mailer/
│
├── index.php               # Main landing and registration page
├── unsubscribe.php         # Handles user unsubscription
└── src/
    ├── functions.php       # Core application logic
    ├── cron.php            # Script executed by the CRON job
    ├── setup_cron.sh       # Script to configure the CRON job
    └── registered_emails.txt # Flat file used to store subscriber emails

