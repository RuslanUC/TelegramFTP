# Telegram-FTP

Use telegram as ftp storage.

Based on [aioftp server](https://github.com/aio-libs/aioftp/blob/master/aioftp/server.py) and [pyrogram](https://github.com/pyrogram/pyrogram).

<details>
<summary><b>Enviroment variables you need to set:</b></summary>

`API_ID`: Go to [my.telegram.org](https://my.telegram.org) to obtain this.

`API_HASH`: Go to [my.telegram.org](https://my.telegram.org) to obtain this.

`BOT_TOKEN`: Get the bot token from [BotFather](https://telegram.dog/botfather).

`MONGODB`: MongoDB connect string.

`CHAT_ID`: Chat id to send files to.

`HOST`: FTP server host (default: 0.0.0.0).

`PORT`: FTP server port (default: 9021).

</details>

<details>
<summary><b>Setup:</b></summary>

  1. Create bot in [BotFather](https://telegram.dog/botfather).
  2. Obtain API_ID and API_HASH on [my.telegram.org](https://my.telegram.org).
  3. Create mongodb database on [MongoDB Cloud](https://cloud.mongodb.com/) (or use your server) and copy connect string.
  4. Insert all variables into .env
  5. Add bot to your channel with admin rights.
  6. Run `get_channel_id.py`, send `/id` command in your channel.
  7. Copy id to .env
  8. Create mongodb database named `ftp`.
  9. Run `setup_database.py`.
  10. Run `create_accounts.py` to create accounts.
  11. Run `main.py`.

</details>