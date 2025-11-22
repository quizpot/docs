---
title: Instalace
sidebar_position: 3
---

Průvodce, jak nainstalovat a spustit Quizpot na vašem zařízení.

### Nainstalujte Git a Node.js

```sh
# Debian/Ubuntu
sudo apt-get install git nodejs

# Fedora/CentOS
sudo dnf install git nodejs

# Arch Linux
sudo pacman -S git nodejs
```

### Naklonujte repozitář

```sh
git clone https://github.com/quizpot/quizpot.git
```

### Přejděte do repozitáře

```sh
cd quizpot
```

### Zkopírujte soubor .env.example do .env

```sh
cp .env.example .env
```

### Upravte soubor .env

Otevřete soubor .env ve svém textovém editoru `Např: nano .env` a upravte následující řádky:

```bash title=".env"
NEXT_PUBLIC_WS_URL=ws://localhost:3000/api/ws # Nahraďte `localhost:3000` s URL, kterou budete používat pro přístup ke své instanci Quizpotu
NEXT_PUBLIC_GEMINI_KEY=key # Volitelné: Nahraďte `key` vaším Gemini API klíčem, který můžete získat z https://aistudio.google.com
NEXT_PUBLIC_PIXABAY_KEY=key # Volitelné: Nahraďte `key` vaším Pixabay API klíčem, který můžete získat z https://pixabay.com/api/docs/ (Nachází se v tabulce parametrů po přihlášení)

# Volitelné: Pro analytiku od Umami
NEXT_PUBLIC_UMAMI_URL=https://umami.example.com 
NEXT_PUBLIC_UMAMI_ID=id
```

> Poznámka: Pokud volitelné proměnné nepotřebujete, odstraňte jejich hodnoty nebo celé řádky.

### Nainstalujte závislosti

```sh
npm install
```

### Sestavte aplikaci

```sh
npm run build
```

### Spusťte aplikaci v produkčním režimu

```sh
npm run start
```

### Otevřete aplikaci ve vašem prohlížeči

Otevřete http://localhost:3000 ve vašem prohlížeči.