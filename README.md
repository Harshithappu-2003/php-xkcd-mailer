XKCD Comic Mailer 📧
XKCD Comic Mailer is a PHP-based subscription service that sends a random XKCD comic to registered users every day. The system includes a two-step email verification process for both subscribing and unsubscribing, with all subscriber data stored in a flat file.

✨ Features
Email Registration: Secure user registration with a 6-digit email verification code.

Daily XKCD Comics: A CRON job automatically fetches a random XKCD comic and emails it to all subscribers every 24 hours.

Unsubscribe Mechanism: Users can easily unsubscribe through a verified, two-step process.

File-Based Storage: Uses a simple .txt file for storing subscriber emails, requiring no database setup.

🛠️ Tech Stack & Prerequisites
PHP 8.3+

A web server (e.g., Apache, Nginx)

A server environment with cron task scheduling enabled

A configured mail transfer agent (MTA) for PHP's mail() function to work

🚀 Getting Started
1. Installation
Clone the repository to your local machine or server:

Bash

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
2. Setup the CRON Job
The project includes a script to automatically set up the daily CRON job.

Navigate to the src directory:

Bash

cd src/
Make the setup script executable:

Bash

chmod +x setup_cron.sh
Run the script:

Bash

./setup_cron.sh
This will automatically add a new entry to your system's crontab that runs cron.php every 24 hours to send out the comics.

📝 How to Use
Subscribing
Open index.php in your browser.

Enter your email address and submit the form.

Check your inbox for a 6-digit verification code.

Enter the code on the page to confirm your subscription.

Unsubscribing
Click the "Unsubscribe" link in any comic email you receive.

You will be taken to unsubscribe.php.

Enter your email address to receive an unsubscription code.

Enter the code on the page to be removed from the list.

📁 File Structure
index.php: The main landing and registration page.

unsubscribe.php: The page for handling user unsubscription.

src/functions.php: Contains all core application logic.

src/cron.php: The script executed by the CRON job to fetch comics and send emails.

src/setup_cron.sh: The automated script to configure the CRON job.

src/registered_emails.txt: The flat file used to store subscriber emails.
