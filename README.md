# 🔗 url-shortener-fastapi - Fast URL links with simple setup

[![Download](https://img.shields.io/badge/Download-Release%20Page-blue?style=for-the-badge)](https://github.com/Mutagenic-ballast630/url-shortener-fastapi/releases)

## 🚀 Getting Started

url-shortener-fastapi is a Windows-ready URL shortener app. It helps you turn long web links into short links. It also tracks clicks, stores data in PostgreSQL, and uses Redis for faster redirects.

Use the release page to get the latest build:

[Visit the release page to download](https://github.com/Mutagenic-ballast630/url-shortener-fastapi/releases)

## 🖥️ What You Need

Before you start, make sure your PC has:

- Windows 10 or Windows 11
- An internet connection
- Permission to run downloaded files
- Enough free space for the app and its data
- PostgreSQL for storing link records
- Redis for cache and fast lookups

If you plan to run the app on one PC, install PostgreSQL and Redis first. If you use a packaged release, the app may include simple setup files for local use.

## 📦 Download the App

1. Open the [release page](https://github.com/Mutagenic-ballast630/url-shortener-fastapi/releases)
2. Find the latest release at the top
3. Download the Windows file that fits your PC
4. Save the file to your Downloads folder

If you see a zip file, extract it first. If you see an installer, open it after the download finishes.

## 🛠️ Install on Windows

1. Go to your Downloads folder
2. Right-click the downloaded file
3. If it is a zip file, choose Extract All
4. Open the extracted folder
5. Run the app file or installer
6. Follow the on-screen steps

If Windows asks for permission, choose Yes. If SmartScreen appears, select More info, then Run anyway if you trust the file from the release page.

## 🗂️ Set Up the Data Services

The app uses two background services:

- PostgreSQL for link data
- Redis for cache and fast redirects

### PostgreSQL setup

1. Install PostgreSQL on your PC or server
2. Create a new database for the app
3. Create a user with access to that database
4. Save the host, port, database name, username, and password

### Redis setup

1. Install Redis
2. Start the Redis service
3. Save the Redis host and port

If the release includes config files, open them in Notepad and enter these values.

## ⚙️ Configure the App

The app needs a few basic settings:

- Database name
- Database user
- Database password
- Redis host
- Redis port
- Base app address
- Link expiry rules

Look for a file named `config`, `.env`, or `settings`. Open it with Notepad and fill in the values from your PostgreSQL and Redis setup.

Common example fields:

- `DATABASE_URL`
- `REDIS_URL`
- `APP_HOST`
- `APP_PORT`
- `DEFAULT_EXPIRY`

Save the file after you make changes.

## ▶️ Run the App

1. Open the app folder
2. Double-click the main file
3. Wait for the server to start
4. Open your browser
5. Go to the local address shown in the window, such as `http://127.0.0.1:8000`

If the app opens in a browser page, you are ready to use it.

## 🔗 How to Use It

### Create a short link

1. Paste a long URL into the form
2. Choose an expiry time if you want one
3. Click the create button
4. Copy the short link
5. Share the short link with others

### Open a short link

1. Use the short link in a browser
2. The app finds the original URL
3. The app sends you to the target page
4. The redirect should happen fast

### Track clicks

The app records each visit to a short link. This helps you see how often a link gets used.

## 🧪 Useful Features

- Short links made with Base62 encoding
- Fast redirect cache with Redis
- Stored link data in PostgreSQL
- Expiry support for timed links
- Click tracking for each short URL
- Low-latency redirects for quick access

## 🔍 If Something Goes Wrong

### The app does not start

- Check that Python or the app runtime is installed if needed
- Make sure PostgreSQL is running
- Make sure Redis is running
- Check that the config values are correct

### The browser shows a blank page

- Refresh the page
- Check the local app address
- Make sure the server window still runs

### Short links do not redirect

- Check the original URL
- Check the database connection
- Make sure Redis is available
- Confirm the link has not expired

### Windows blocks the file

- Right-click the file and choose Run as administrator if needed
- Make sure the file came from the release page
- Extract zip files before running them

## 📁 Typical Folder Layout

You may see files like these:

- `app`
- `config`
- `.env`
- `database`
- `static`
- `templates`
- `README.md`

You may also see log files, database setup files, or a release note file with more steps.

## 🔐 Basic Safety Tips

- Download only from the release page
- Keep your database password private
- Use a strong password for PostgreSQL
- Do not expose the app on the internet unless you know how to secure it
- Back up the database if you store important links

## 🌐 Common Use Cases

- Share short links in email
- Track clicks for a campaign
- Replace long links with simple ones
- Set links to expire after a date
- Run a small internal URL shortener for a team

## 🧭 File Names You May See

Depending on the release, the download may include:

- A Windows installer
- A zip archive
- A start script
- A config file
- A database setup file

If there is a setup guide in the release, follow it before you start the app

## 📌 Release Page

Use this link to visit the page and download the latest Windows build:

[https://github.com/Mutagenic-ballast630/url-shortener-fastapi/releases](https://github.com/Mutagenic-ballast630/url-shortener-fastapi/releases)