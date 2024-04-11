# SparkyH1BDropBoxAlert

## Overview
SparkyH1BDropBoxAlert is a Python script designed to monitor specific Telegram chats for messages containing available appointment slots for H1B and H4 visa processing, then alert users via email, push notification and Alexa notifications.

```
Frustration + ChatGpt + Python + free time + innovation = My tool to alert me --> Booked my slots in Jun on 10-Apr after running this script 24x7 for two weeks. Chat with ChatGPT if you are stuck anywhere or message me if you need any help with confiugration. 
```

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
  https://support.google.com/mail/answer/185833?hl=en
- An Alexa device with Notify Me and Voice Monkey skills for voice notifications.
    -   https://www.amazon.com/Thomptronics-Notify-Me/dp/B07BB2FYFS
    -   https://www.amazon.com/TopVoiceApps-com-Voice-Monkey/dp/B08C6Z4C3R
-  IFFT configuration
    - Create an account in IFFT, install its mobile app.
    - Create an Applet in web version with EMAIL. Whenever you receive email to IFFT from your registered email, setup push notication. Make sure to use the same SMTP email used in previous step in here as well. Otherwise push notication will not work. 
   ![image](https://github.com/CodeWithCJ/SparkyH1BDropBoxAlert/assets/151883488/549a3fb6-23eb-4bdd-a299-eb6dd773dd84)



## Configuration
1. **Telegram API**: Sign up for Telegram API access and obtain your `api_id` and `api_hash`. Replace `your_telegram_app_id` and `your_telegram_app_hash` in the `config.ini` with your actual Telegram API credentials.
2. **SMTP Settings**: Replace `youremail@gmail.com` and `your_smtp_password` in the `config.ini` with your actual email and password that will be used to send notifications.
3. Configure IFFT Applet with same email ID to receive push notication - Refer Wiki page for more detailed instruction. 
4. **Alexa Notify Me**: Set up Alexa Notify Me and obtain your access code. Replace `your_Alexa_notifify_me_access_code` in the `config.ini` with your actual Notify Me access code.
5. **Alexa Voice Monkey**: Set up Voice Monkey for your Alexa device and obtain the URL. Replace `your_Alex_Voice_Monekey_URL` in the `config.ini` with your actual Voice Monkey URL. Refer WIKI page for detailed instruction 

```
Step 3 to 5 are optional. But highly recommend configuring at least one otherwise, high chance you will the alert.
```

## Installation
To install the required Python libraries, run the following command:
```bash
pip install -r requirements.txt
```

## How to Run
```bash
python SparkyH1BDropBoxAlert.py
```
