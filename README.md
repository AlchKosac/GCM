# GamingConnectionMonitor (GCM)

**Česky** · [English](#english)

Desktopová aplikace pro hráče na Windows, která hlídá kvalitu připojení k hrám:

- **Trasa** – průběžné měření latence, jitteru a ztrát na každém routeru (hopu) cesty k cíli, graf v čase a srozumitelný rozbor, kde je problém (u vás, u operátora, nebo u herního serveru).
- **Herní služby** – oficiální stav her a platforem (Xbox Live, PlayStation Network, Epic Games, Riot Games, EVE Online, Discord…) a vlastní měření dostupnosti; hry se přidávají vyhledáváním z připravených profilů.
- **Xbox / NAT** – typ NAT, UPnP, Teredo a služby Windows potřebné pro hraní přes Xbox aplikaci.
- **Stahování na pozadí** – které programy a služby Windows (Windows Update, Microsoft Store, Steam…) právě stahují, kolik a z jakého serveru, upozornění při hře a volitelné omezení rychlosti stahování Windows po dobu hry.
- **Provoz hry** – přenos dat spuštěné hry, herní server, zastavení toku a porovnání s měřenou trasou.
- **Nástroje** – test rychlosti s bufferbloatem, rychlá kontrola a oprava DNS, hlídání výpadků DNS, stav linky, nastavení sítě a veřejná IP s historií.

$1
## Ukázky

![Přehled – stav služeb, trasa, stahování na pozadí a provoz hry](docs/prehled.png)

![Trasa – měření latence a ztrát na každém hopu s grafem a rozborem](docs/trasa.png)

## Stažení

**[⬇ Stáhnout GCM (ZIP, nejnovější verze)](https://github.com/AlchKosac/GCM/releases/latest/download/GCM-win64.zip)** – rozbalte a spusťte `gcm.exe` ze složky „GCM - GamingConnectionMonitor“, nic se neinstaluje (Windows 10 / 11). Přehled verzí a novinek je v sekci [Releases](../../releases). Další verze aplikace nabídne sama (automatická aktualizace).

Při prvním spuštění může Windows zobrazit varování SmartScreen (aplikace zatím není digitálně podepsaná) – zvolte „Další informace“ › „Přesto spustit“.
Nastavení a naměřená data se ukládají do `%APPDATA%\GCM` – vedle `gcm.exe` aplikace nic nevytváří, složku můžete přesunout kamkoli.

## Co je v tomto repozitáři

| Složka | Obsah |
|---|---|
| `profiles/games.json` | profily her a služeb – odkud aplikace bere oficiální stav, co měří a proč. Aplikace si je jednou denně stáhne, takže nové hry a opravy přibývají bez nové verze aplikace. |
| `lang/*.json` | překlady do dalších jazyků |
| [Releases](../../releases) | spustitelné `gcm.exe` |

Zdrojový kód aplikace zde není.

## Kontakt a podpora

Novinky, dotazy a návrhy: [Discord GuildAgenda](https://discord.gg/d6a4rkB666).

Aplikace je zdarma. Autor: Kosáč.

---

## English

A Windows desktop app for gamers that monitors connection quality:
per-hop latency / jitter / loss tracing with a plain-language analysis, official status of games and platforms
plus own reachability checks (games are added by searching ready-made profiles), Xbox NAT / Teredo diagnostics,
speed test with bufferbloat, DNS check and repair, DNS outage monitoring, link / Wi-Fi status, network settings with public IP history, per-program background download monitoring with notifications while gaming, and an optional limit for Windows downloads during a game. Available in Czech, Slovak and English.

**[Download GCM (ZIP, latest)](https://github.com/AlchKosac/GCM/releases/latest/download/GCM-win64.zip)** – unzip and run `gcm.exe` (see [Releases](../../releases)) (Windows 10 / 11, no installation). Settings and data are stored in `%APPDATA%\GCM`.
This repository contains the game profiles (`profiles/games.json`, downloaded by the app daily), translations (`lang/`)
and releases – not the source code. Contact: [Discord](https://discord.gg/d6a4rkB666).
