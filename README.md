
# Truecaller and Smsbomber telegram bot

This bot can provide you Truecaller and Smsbomber features using api requests

Made using [python_telegram_bot](https://github.com/python-telegram-bot/python-telegram-bot)





## Requirements


You can Install requirements using
```sh
pip install -r requirements.txt
```


## Usage

To get you bot Api Key

Go to Telegram app and search '@BotFather' 

Click on /newbot

Give your bot a name and a username and your Done!

Add your api_key to environment variable and add it to line 12.
or replace the line with api_key = actual api key


## Heroku Guide For Webhook Version

1. Create a webhook with link below

```bash
   https://api.telegram.org/bot{ your api key }/setwebhook?url=https://{ your heroku app name }.herokuapp.com
```
2. You will see a success message saying webhook was setup

3. Go to main_webhook.py and add your api key at line 13 and your heroku app name at line 124



For the webhook version you need to scale your dynos

```bash
    heroku ps:scale web=1 -a your_heroku_app_name
```

