# SparkyH1BDropBoxAlert

## Overview
SparkyH1BDropBoxAlert is a Python script designed to monitor specific Telegram chats for messages containing available appointment slots for H1B and H4 visa processing, then alert users via email, push notification and Alexa notifications.

## Prerequisites
Before you can run this script, you will need:
- Python 3.x installed on your system.
- A Telegram account with API access.
- An SMTP server (Gmail used in this example) for sending emails.
- An Alexa device with Notify Me and Voice Monkey skills for voice notifications.

## Configuration
1. **Telegram API**: Sign up for Telegram API access and obtain your `api_id` and `api_hash`. Replace `your_telegram_app_id` and `your_telegram_app_hash` in the `config.ini` with your actual Telegram API credentials.
2. **SMTP Settings**: Replace `youremail@gmail.com` and `your_smtp_password` in the `config.ini` with your actual email and password that will be used to send notifications.
3. **Alexa Notify Me**: Set up Alexa Notify Me and obtain your access code. Replace `your_Alexa_notifify_me_access_code` in the `config.ini` with your actual Notify Me access code.
4. **Alexa Voice Monkey**: Set up Voice Monkey for your Alexa device and obtain the URL. Replace `your_Alex_Voice_Monekey_URL` in the `config.ini` with your actual Voice Monkey URL.

## Installation
To install the required Python libraries, run the following command:
```bash
pip install -r requirements.txt
