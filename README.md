# Telegram MediaLibrary-Bot Bot

A Telegram bot that allows admins to upload films, cartoons, or anime and store their Telegram `file_id` in a PostgreSQL database. Users can search media by **name or ID** and receive the content directly from the bot.

---

## Features
- Admin-only media upload (films, cartoons, anime)
- Stores Telegram `file_id` and metadata in PostgreSQL
- Search media by name or unique ID
- Channel membership check before allowing access
- Post publishing with inline buttons linking to media
- User statistics (total users, active users)
- Referral & contest system (tracks invited users)
- Deployed online using Alwaysdata and neon.tech

---

## Tech Stack
- Python
- telebot (pyTelegramBotAPI)
- PostgreSQL
- Alwaysdata
- neon.tech
- GitHub

---

## How It Works
1. Admin uploads media files to the bot
2. Bot saves `file_id` and related data to PostgreSQL
3. User searches media by name or ID
4. Bot checks channel membership
5. Bot sends the requested media

---

## Installation
```bash
pip install -r requirements.txt
python bot.py
```

----

## Deployment
The bot is deployed using **alwaysdata**.
- works with SSH keys
- Supports webhook or polling mode
- Automatically restarts on failure

---

## Database Setup
The bot uses **PostgreSQL** to store media file IDs, user data, and referral statistics.

- Database connection is managed via environment variables
- Tables are created automatically on first run
- Compatible with cloud PostgreSQL services (e.g., Neon, Supabase)

---

##Notes
Bot .env file for bot API and username.

