# Telegram Reminder Bot
A Telegram Bot which serves as a reminder for your meetings, appointments, events etc.

```/start -> add a new reminder```

```/list -> lists all scheduled future reminders```

```/time -> change your timezone (standard on utc time)```

## Try the bot
You can use the bot under: http://t.me/Appointment_Reminder_Bot

## How it works
The code uses the telegram.ext ConversationHandler to create a guided and flawless conversation flow. Moreover it uses different other telegram.ext classes
to "ask & get" the responses information from the user. Furthermore all of the data is being stored in [reminder.json]
to create the data flow between the different states of the ConversationHandler and have the opportunity to access the reminder later on (e.g. for the ```/list``` command).
To provide this bot for people from different timezones, you have the opportunity to set your local timezone using the ```/time``` command to receive the reminders for your local time instead of the bot's / server's local time.
Disclaimer: This is my first bot for telegram, so there might be things that could have been implemented and routed easier than I did.