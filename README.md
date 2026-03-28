<h1 align="center">InfinityGamer FileStreamBot</h1>
<p align="center">
  <a href="https://github.com/infinitygamer/FileStreamBot">
    <img src="https://graph.org/file/80d1f94e81bbc1acadb36.jpg" alt="Cover Image" width="550">
  </a>
</p>  
<p align="center">
  <br><b>
    <a href="https://github.com/infinitygamer/FileStreamBot/issues">Report a Bug</a>
    |
    <a href="https://github.com/infinitygamer/FileStreamBot/issues">Request Feature</a>
  </b>
</p>

---

### 🍁 About :

<p align="center">
    <a href="https://github.com/infinitygamer/FileStreamBot">
        <img src="https://i.ibb.co/ZJzJ9Hq/link-3x.png" height="100" width="100" alt="FileStreamBot Logo">
    </a>
</p>
<p align='center'>
  This bot provides stream links for Telegram files without the necessity of waiting for the download to complete, offering the ability to store files. <br>
  <b>Customized & maintained by InfinityGamer</b>
</p>

---

### ♢ How to Deploy :

<i>Either you could locally host, VPS, or deploy on Railway / Render</i>

#### ♢ Click on This Drop-down and get more details

<br>
<details>
  <summary><b>Deploy Locally :</b></summary>
<br>

```sh
git clone https://github.com/infinitygamer/FileStreamBot
cd FileStreamBot
python3 -m venv ./venv
. ./venv/bin/activate
pip install -r requirements.txt
python3 -m FileStream
```

* To stop the whole bot,
  do <kbd>CTRL</kbd>+<kbd>C</kbd>

* If you want to run this bot 24/7 on the VPS, follow these steps.

```sh
sudo apt install tmux -y
tmux
python3 -m FileStream
```

* now you can close the VPS and the bot will run on it.

</details>

---

<details>
  <summary><b>Deploy using Docker :</b></summary>
<br>

```sh
git clone https://github.com/infinitygamer/FileStreamBot
cd FileStreamBot
docker build -t file-stream .
docker run -d --restart unless-stopped --name fsb \
-v /PATH/TO/.env:/app/.env \
-p 8000:8000 \
file-stream
```

</details>

---

<details>
  <summary><b>Setting up things :</b></summary>

Create a `.env` file:

```sh
API_ID = 123456
API_HASH = your_api_hash
BOT_TOKEN = your_bot_token
ULOG_CHANNEL = -100xxxxxxxx
FLOG_CHANNEL = -100xxxxxxxx
DATABASE_URL = your_mongodb_url
FQDN = your_domain
HAS_SSL = True
OWNER_ID = your_user_id
PORT = 8080
```

</details>

---

<details>
  <summary><b>Vars and Details :</b></summary>

#### 📝 Mandatory Vars :

* `API_ID` - Telegram API ID
* `API_HASH` - Telegram API Hash
* `BOT_TOKEN` - Bot Token from BotFather
* `OWNER_ID` - Your Telegram ID
* `FLOG_CHANNEL` - Storage Channel
* `ULOG_CHANNEL` - Logs Channel
* `DATABASE_URL` - MongoDB URL
* `FQDN` - Your domain

</details>

---

<details>
  <summary><b>How to Use :</b></summary>

#### Bot Commands :

```sh
/start
/help
/about
/files
```

</details>

---

### 🚀 Features

* 📁 File → Link Generator
* 🎬 Streaming Support
* ⚡ Fast downloads
* 🌐 Works in browser
* 💾 MongoDB storage

---

### 👑 Owner

<p align="center">
<b>InfinityGamer</b>
</p>

---

<h4 align='center'>© 2026 InfinityGamer</h4>
