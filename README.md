# 🛡️ Telegram Username Enumeration Tool
![Logo](image.jpg)

This Python script automates **username availability checks on Telegram** using the Telegram API.  
It is designed for **OSINT investigations, security audits, and account takeover risk assessment**, allowing security researchers to identify unclaimed usernames for analysis or monitoring.

> ⚠️ **Important:** Use a user account (phone number). Telegram restricts bots from checking usernames.

---

## 🔐 Cybersecurity Use Cases

- **OSINT & reconnaissance**: Collect data about potential usernames for monitoring.  
- **Account takeover risk assessment**: Identify available usernames tied to specific organizations or campaigns.  
- **Security research & testing**: Validate username policy weaknesses or exposure.

---

## ⚙️ Requirements

- Python 3.7+  
- Python packages:
  - `pyrogram`
  - `requests`

Install packages:
```bash
pip install -r requirements.txt
```
## 📌 Telegram API Credentials
```
Register an application at my.telegram.org
 to obtain:

 API ID: Your API ID
API Hash: Your API Hash
Bot Token: Create a bot using BotFather
Chat ID: Use @userinfobot to find your chat ID
Update the script with your credentials before running.
```
## 🚀 Usage
```
Clone repository and install requirements:

git clone https://github.com/ghostuser-bug/telegram-username-enum.git
cd telegram-username-enum
pip install -r requirements.txt

```
Create words.txt in the same directory with usernames to check, one per line.

Update credentials in checker.py:

api_id = YOUR_API_ID
api_hash = 'YOUR_API_HASH'
bot_token = 'YOUR_BOT_TOKEN'
chat_id = 'YOUR_CHAT_ID'


Run the script:

python checker.py

The script checks each username from words.txt.

Sends a message to your Telegram chat if a username is available.

Pauses 10 seconds between checks to avoid hitting Telegram rate limits.

⚠️ Legal Disclaimer
```
Use responsibly. Unauthorized enumeration or monitoring of accounts without consent may violate Telegram's terms of service or local laws. This tool is intended for authorized security research and OSINT activities.
```
