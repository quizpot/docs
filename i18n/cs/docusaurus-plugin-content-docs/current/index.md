---
sidebar_position: 1
title: Představení
slug: /
---

# Představení

Quizpot je aplikace, která umožňuje vytvářet kvízy bez omezení, na vlastní podmínky.

## Požadavky

* 2 CPU Jádra
* ~2 GB RAM
* 2 GB Úložiště

> [Detailní požadavky](/requirements)

## Rychlý Start

Spusťte Quizpot snadno pomocí následujících příkazů:

> Poznámka: Toto předpokládá, že máte na svém zařízení nainstalované závislosti. [Pokud ne, postupujte podle pokynů zde](/installation)

```sh
# Naklonujte repozitář
git clone https://github.com/quizpot/quizpot.git

# Přejděte do repozitáře
cd quizpot

# Zkopírujte soubor .env.example do .env
cp .env.example .env

# Nainstalujte a spusťte aplikaci ve vývojovém režimu
npm install && npm run dev
```
