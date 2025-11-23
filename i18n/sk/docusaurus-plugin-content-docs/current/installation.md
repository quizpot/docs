---
title: Inštalácia
sidebar_position: 3
---

Sprievodca, ako nainštalovať a spustiť Quizpot na vašom zariadení.

### Nainštalujte Git a Node.js

```sh
# Debian/Ubuntu
sudo apt-get install git nodejs

# Fedora/CentOS
sudo dnf install git nodejs

# Arch Linux
sudo pacman -S git nodejs
```

### Naklonujte repozitár

```sh
git clone https://github.com/quizpot/quizpot.git
```

### Prejdite do repozitára

```sh
cd quizpot
```

### Prejdite do repozitára

```sh
cp .env.example .env
```

### Upravte súbor .env

Otvorte súbor .env vo svojom textovom editore `Napr: nano .env` a upravte nasledujúce riadky:

```bash title=".env"
NEXT_PUBLIC_WS_URL=ws://localhost:3000/api/ws # Nahraďte `localhost:3000` s URL, ktorú budete používať na prístup k vašej inštancii Quizpotu
NEXT_PUBLIC_PIXABAY_KEY=key # Voliteľné: Nahraďte `key` vaším Pixabay API kľúčom, ktorý môžete získať z https://pixabay.com/api/docs/ (Nachádza sa v tabuľke parametrov po prihlásení)

# Voliteľné: Pre analytiku od Umami
NEXT_PUBLIC_UMAMI_URL=https://umami.example.com 
NEXT_PUBLIC_UMAMI_ID=id

GEMINI_KEY=key # Voliteľné: Nahraďte `key` vaším Gemini API kľúčom, ktorý môžete získať z https://aistudio.google.com
```

> Poznámka: Odstráňte hodnoty alebo celé riadky voliteľných premenných, ak ich nepotrebujete.

### Nainštalujte závislosti

```sh
npm install
```

### Zostavte aplikáciu

```sh
npm run build
```

### Spustite aplikáciu v produkčnom režime

```sh
npm run start
```

### Otvorte aplikáciu vo vašom prehliadači

Otvorte http://localhost:3000 vo vašom prehliadači.