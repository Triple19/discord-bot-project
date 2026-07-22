**Please Read this file to know how to run the project and contribute.

#### **How to Set Up the Discord Bot**

Welcome! This guide will walk you through everything you need to get the Discord bot running on your computer. Even if you've never worked with Python or a Discord bot before, following these steps should get you up and running.

Before You Begin

Before you can run the bot, you'll need a few programs installed on your computer.

Required Software
Python

Python is the programming language used to build this bot.

Download the latest version from:

https://www.python.org/downloads/

Important: During installation, make sure to check the box labeled "Add Python to PATH" before clicking Install Now. This allows you to run Python commands from the terminal.

Visual Studio Code

Visual Studio Code (VS Code) is the code editor we will use to write and edit the bot.

Download it here:

https://code.visualstudio.com/

Git

Git allows everyone on the team to work on the same project without overwriting each other's work.

Download Git here:

https://git-scm.com/downloads

Downloading the Project

There are two ways to get the project onto your computer.

## Option 1 (Recommended)

Clone the repository using Git.

Open a terminal and run:

git clone <repository link>

This downloads the latest version of the project.

## Option 2

Go to the GitHub repository.

Click the green Code button.

Select Download ZIP.

Extract the ZIP file somewhere easy to find.

#### **Opening the Project**
Open Visual Studio Code.
Click File → Open Folder.
Select the Discord Bot project folder.

You should now see all of the project files on the left side of VS Code.

Installing the Required Packages

The bot depends on several Python libraries that are not included with Python.

These libraries are listed inside requirements.txt.

Open a terminal in VS Code by clicking:

Terminal → New Terminal

Then run:

**pip install -r requirements.txt**

This command automatically downloads every required dependency for the project.

You only need to do this once (or whenever new dependencies are added).

Setting Up the Discord Token

Discord bots require a secret token to log into Discord.

You should already have a file named:

.env.example

Copy this file and rename the copy to:

.env

Open the .env file.

Replace the placeholder with your bot token.

Example:

DISCORD_TOKEN=YOUR_BOT_TOKEN_HERE

Never upload your .env file to GitHub.

It contains private information.

Running the Bot

Once everything has been installed, start the bot by running:

python bot.py

If everything is working correctly, you should see a message similar to:

Bot is online!

Your bot should now appear online in your Discord server.

Project Structure

Our project is organized so everyone can work independently.

discord-bot/
│
├── bot.py
├── config.py
├── commands/
├── utils/
├── requirements.txt
├── README.md
└── HOW_TO_SETUP.md
bot.py

The main file of the project.

This starts the bot, loads commands, and connects to Discord.

config.py

Stores project settings such as the Discord token and future configuration values.

commands/

Contains all of the bot's commands.

Each file groups similar commands together.

Example:

utility.py
moderation.py
fun.py
information.py

When adding a new command, make sure it belongs in the correct file.

utils/

Contains helper functions that multiple commands can use.

Examples include:

Creating embeds
Formatting messages
Shared utility functions
Basic Development Workflow

Whenever you work on the project, follow this process:

Pull the latest version from GitHub.
Make your changes.
Test your changes.
Save your work.
Commit your changes.
Push your changes back to GitHub.

Following this workflow helps prevent merge conflicts and ensures everyone is working with the latest code.

Basic Git Commands

Download the latest version:

git pull

Stage your changes:

git add .

Create a commit:

git commit -m "Describe your changes"

Upload your work:

git push

Always pull before beginning work.

Common Terminal Commands
Command	Description
cd foldername	Move into a folder
cd ..	Move back one folder
dir (Windows) / ls (macOS/Linux)	View files in the current folder
pip install -r requirements.txt	Install project dependencies
python bot.py	Start the bot
git pull	Download the latest project changes
git push	Upload your changes
Troubleshooting
"Python is not recognized"

Python is either not installed or was not added to your system's PATH during installation.

Reinstall Python and ensure "Add Python to PATH" is selected.

"No module named..."

One or more required packages are missing.

Run:

pip install -r requirements.txt
The bot will not start

Check the terminal for any error messages.

Verify that:

Python is installed.
All dependencies have been installed.
Your .env file contains a valid bot token.
Slash commands are missing

Restart the bot.

It may take a minute or two for Discord to synchronize new slash commands.**# How to Set Up the Discord Bot

> **Please read this guide before contributing to the project.**
>
> This document explains how to set up the Discord bot, run it on your computer, and contribute to the project.

---

# Before You Begin

Before you can run the bot, you'll need a few programs installed on your computer.

## Required Software

### Python

Python is the programming language used to build this bot.

Download the latest version from:

https://www.python.org/downloads/

> **Important:** During installation, make sure to check **"Add Python to PATH"** before clicking **Install Now**. This allows you to run Python commands from the terminal.

---

### Visual Studio Code

Visual Studio Code (VS Code) is the code editor we will use to write and edit the bot.

Download it here:

https://code.visualstudio.com/

---

### Git

Git allows everyone on the team to work on the same project without overwriting each other's work.

Download it here:

https://git-scm.com/downloads

---

# Downloading the Project

There are two ways to download the project.

## Option 1 (Recommended)

Clone the repository using Git.

Open a terminal and run:

```bash
git clone <repository link>
```

This downloads the latest version of the project.

---

## Option 2

1. Go to the GitHub repository.
2. Click the green **Code** button.
3. Select **Download ZIP**.
4. Extract the ZIP file somewhere easy to find.

---

# Opening the Project

1. Open **Visual Studio Code**.
2. Click **File → Open Folder**.
3. Select the Discord Bot project folder.

You should now see all of the project files on the left side of VS Code.

---

# Installing the Required Packages

The bot depends on several Python libraries that are not included with Python.

These libraries are listed inside **requirements.txt**.

Open a terminal in VS Code by clicking:

**Terminal → New Terminal**

Then run:

```bash
pip install -r requirements.txt
```

This command automatically downloads every required dependency for the project.

> You only need to do this once (or whenever new dependencies are added).

---

# Setting Up the Discord Token

Discord bots require a secret token to log into Discord.

You should already have a file named:

```text
.env.example
```

Copy this file and rename the copy to:

```text
.env
```

Open the `.env` file.

Replace the placeholder with your bot token.

Example:

```env
DISCORD_TOKEN=YOUR_BOT_TOKEN_HERE
```

> **Never upload your `.env` file to GitHub.**
>
> It contains private information.

---

# Running the Bot

Once everything has been installed, start the bot by running:

```bash
python bot.py
```

If everything is working correctly, you should see a message similar to:

```text
Bot is online!
```

Your bot should now appear online in your Discord server.

---

# Project Structure

Our project is organized so everyone can work independently.

```text
discord-bot/
│
├── bot.py
├── config.py
├── commands/
├── utils/
├── requirements.txt
├── README.md
└── HOW_TO_SETUP.md
```

## bot.py

The main file of the project.

This starts the bot, loads commands, and connects to Discord.

---

## config.py

Stores project settings such as the Discord token and future configuration values.

---

## commands/

Contains all of the bot's commands.

Each file groups similar commands together.

Example:

- utility.py
- moderation.py
- fun.py
- information.py

When adding a new command, make sure it belongs in the correct file.

---

## utils/

Contains helper functions that multiple commands can use.

Examples include:

- Creating embeds
- Formatting messages
- Shared utility functions

---

# Basic Development Workflow

Whenever you work on the project, follow this process:

1. Pull the latest version from GitHub.
2. Make your changes.
3. Test your changes.
4. Save your work.
5. Commit your changes.
6. Push your changes back to GitHub.

Following this workflow helps prevent merge conflicts and ensures everyone is working with the latest code.

---

# Basic Git Commands

### Download the latest version

```bash
git pull
```

---

### Stage your changes

```bash
git add .
```

---

### Create a commit

```bash
git commit -m "Describe your changes"
```

---

### Upload your work

```bash
git push
```

> **Always pull before beginning work.**

---

# Common Terminal Commands

| Command | Description |
|----------|-------------|
| `cd foldername` | Move into a folder |
| `cd ..` | Move back one folder |
| `dir` (Windows) / `ls` (macOS/Linux) | View files in the current folder |
| `pip install -r requirements.txt` | Install project dependencies |
| `python bot.py` | Start the bot |
| `git pull` | Download the latest project changes |
| `git push` | Upload your changes |

---

# Troubleshooting

## "Python is not recognized"

Python is either not installed or was not added to your system's PATH during installation.

Reinstall Python and ensure **"Add Python to PATH"** is selected.

---

## "No module named..."

One or more required packages are missing.

Run:

```bash
pip install -r requirements.txt
```

---

## The bot will not start

Check the terminal for any error messages.

Verify that:

- Python is installed.
- All dependencies have been installed.
- Your `.env` file contains a valid bot token.

---

## Slash commands are missing

Restart the bot.

It may take a minute or two for Discord to synchronize new slash commands.

---

# Final Tips

- Pull the latest changes before starting work.
- Test every new command before pushing your code.
- Keep related commands inside the appropriate file.
- Never commit your `.env` file.
- Write clear commit messages.
- Ask questions if you're unsure before making major changes.

---

# Helpful Resources

- **Python Documentation**  
  https://docs.python.org/3/

- **discord.py Documentation**  
  https://discordpy.readthedocs.io/

- **Discord Developer Portal**  
  https://discord.com/developers/applications

- **Discord API Documentation**  
  https://discord.com/developers/docs

- **Visual Studio Code Documentation**  
  https://code.visualstudio.com/docs

- **Git Documentation**  
  https://git-scm.com/docs
