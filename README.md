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


![WhatsApp Image 2025-07-31 at 12 14 16_34c35370](https://github.com/user-attachments/assets/2b193b87-3569-41e6-ad90-22bc56d584f9)
![WhatsApp Image 2025-07-31 at 12 14 16_e647b545](https://github.com/user-attachments/assets/d4339fc3-d568-46b7-9577-824fc65c57cc)
![WhatsApp Image 2025-07-31 at 12 14 17_1a823385](https://github.com/user-attachments/assets/279ef35a-a6f9-4f55-86c2-fdd59c9329aa)
![WhatsApp Image 2025-07-31 at 12 14 19_b09e5535](https://github.com/user-attachments/assets/c3e0fe1a-0296-4340-99eb-69ee120fa4fc)
![WhatsApp Image 2025-07-31 at 12 14 18_999dfef0](https://github.com/user-attachments/assets/51c4a81c-ee49-48d5-8130-9d513d2bc62e)
![WhatsApp Image 2025-07-31 at 12 14 17_89d78377](https://github.com/user-attachments/assets/657ffa9c-fbb1-4b72-a39f-9c450afa5a86)
![WhatsApp Image 2025-07-31 at 12 14 19_46ed5eef](https://github.com/user-attachments/assets/5bad0f48-4eb8-4181-9265-62a8dc180b82)
![WhatsApp Image 2025-07-31 at 12 14 20_a7b09929](https://github.com/user-attachments/assets/4873b3c9-e9de-4b89-b155-e3cf28050760)
![WhatsApp Image 2025-07-31 at 12 14 20_5faea8de](https://github.com/user-attachments/assets/46779bbd-dd2d-42db-b716-da6bdf043602)
![WhatsApp Image 2025-07-31 at 12 14 18_43b3ccc3](https://github.com/user-attachments/assets/a0dd803d-2eeb-48be-8f54-ff7fe9e17947)
