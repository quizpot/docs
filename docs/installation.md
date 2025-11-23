---
title: Installation
sidebar_position: 3
---

Guide on how to install and run Quizpot on your machine.

### Install Git & Node.js

```sh
# Debian/Ubuntu
sudo apt-get install git nodejs

# Fedora/CentOS
sudo dnf install git nodejs

# Arch Linux
sudo pacman -S git nodejs
```

### Clone the repository

```sh
git clone https://github.com/quizpot/quizpot.git
```

### Go into the repository

```sh
cd quizpot
```

### Copy the .env.example file to .env

```sh
cp .env.example .env
```

### Edit the .env file

Open the .env file in your text editor `Ex: nano .env` and edit the following lines:

```bash title=".env"
NEXT_PUBLIC_WS_URL=ws://localhost:3000/api/ws # Replace `localhost:3000` with URL that you will be using to access your Quizpot instance
NEXT_PUBLIC_PIXABAY_KEY=key # Optional: Replace `key` with your Pixabay API key that you can get from https://pixabay.com/api/docs/ (It's located in the parameter table after logging in)

# Optional: For analytics by Umami
NEXT_PUBLIC_UMAMI_URL=https://umami.example.com 
NEXT_PUBLIC_UMAMI_ID=id

GEMINI_KEY=key # Optional: Replace `key` with your Gemini API key that you can get from https://aistudio.google.com
```

> Note: Remove values or whole lines of optional variables if you don't need them.

### Install dependencies

```sh
npm install
```

### Build the application

```sh
npm run build
```

### Run the application in production mode

```sh
npm run start
```

### Open the application in your browser

Open http://localhost:3000 in your browser.