# SparkyH1BDropBoxAlert

## Overview
SparkyH1BDropBoxAlert is a Python script designed to monitor specific Telegram chats for messages containing available appointment slots for H1B and H4 visa processing, then alert users via email, push notification and Alexa notifications.

## Prerequisites
Before you can run this script, you will need:
- Python 3.x
  - Download & install Python using https://www.python.org/downloads/
    - Make sure to install these packages as well. 
        telethon
        pandas
        pytz
        requests
- A Telegram account with API access.
  https://core.telegram.org/api/obtaining_api_id#:~:text=Obtaining%20api_id&text=Sign%20up%20for%20Telegram%20using,parameters%20required%20for%20user%20authorization.
- An SMTP server (Gmail used in this example) for sending emails.
- An Alexa device with Notify Me and Voice Monkey skills for voice notifications.
  https://www.amazon.com/Thomptronics-Notify-Me/dp/B07BB2FYFS
  [https://voicemonkey.io/start](https://www.amazon.com/TopVoiceApps-com-Voice-Monkey/dp/B08C6Z4C3R)
-  IFFT configuration
  -    Create an account in IFFT, install its mobile app.
  -    Create an Applet in web version with EMAIL. Whenever you receive email to IFFT from your registered email, setup push notication. Make sure to use the same SMTP email used in previous step in here as well. Otherwise push notication will not work. 
   ![image](https://github.com/CodeWithCJ/SparkyH1BDropBoxAlert/assets/151883488/549a3fb6-23eb-4bdd-a299-eb6dd773dd84)



## Configuration
1. **Telegram API**: Sign up for Telegram API access and obtain your `api_id` and `api_hash`. Replace `your_telegram_app_id` and `your_telegram_app_hash` in the `config.ini` with your actual Telegram API credentials.
2. **SMTP Settings**: Replace `youremail@gmail.com` and `your_smtp_password` in the `config.ini` with your actual email and password that will be used to send notifications.
3. **Alexa Notify Me**: Set up Alexa Notify Me and obtain your access code. Replace `your_Alexa_notifify_me_access_code` in the `config.ini` with your actual Notify Me access code.
4. **Alexa Voice Monkey**: Set up Voice Monkey for your Alexa device and obtain the URL. Replace `your_Alex_Voice_Monekey_URL` in the `config.ini` with your actual Voice Monkey URL.

## Installation
To install the required Python libraries, run the following command:
```bash
pip install -r requirements.txt
