# GamingConnectionMonitor (GCM)

**Česky** · [English](#english)

Desktopová aplikace pro hráče na Windows, která hlídá kvalitu připojení k hrám:

- **Trasa** – průběžné měření latence, jitteru a ztrát na každém routeru (hopu) cesty k cíli, graf v čase a srozumitelný rozbor, kde je problém (u vás, u operátora, nebo u herního serveru).
- **Herní služby** – oficiální stav her a platforem (Xbox Live, PlayStation Network, Epic Games, Riot Games, EVE Online, Discord…) a vlastní měření dostupnosti; hry se přidávají vyhledáváním z připravených profilů.
- **Xbox / NAT** – typ NAT, UPnP, Teredo a služby Windows potřebné pro hraní přes Xbox aplikaci.
- **Nástroje** – test rychlosti s bufferbloatem, hlídání výpadků DNS, stav linky a Wi-Fi.

Aplikace je v češtině, slovenštině a angličtině.

## Stažení

Aktuální verze je v sekci [Releases](../../releases) – stačí stáhnout `gcm.exe` a spustit (Windows 10 / 11, bez instalace).
Nastavení a naměřená data se ukládají do `%APPDATA%\GCM`.

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
speed test with bufferbloat, DNS outage monitoring and link / Wi-Fi status. Available in Czech, Slovak and English.

Download `gcm.exe` from [Releases](../../releases) (Windows 10 / 11, no installation). Settings and data are stored in `%APPDATA%\GCM`.
This repository contains the game profiles (`profiles/games.json`, downloaded by the app daily), translations (`lang/`)
and releases – not the source code. Contact: [Discord](https://discord.gg/d6a4rkB666).
