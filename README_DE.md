


<h1 align="center">Twitch watcher</h1>
<p align="center"> Ein Bot der autamatisch Twitch Streams anschaut und die Drops sammelt.</p>
<p align="center">
<img alt="GitHub package.json version" src="https://img.shields.io/github/package-json/v/InstreakTV/twitch-watcher"> <img alt="GitHub" src="https://img.shields.io/github/repo-size/InstreakTV/twitch-watcher"> <img alt="GitHub repo size" src="https://img.shields.io/github/license/InstreakTV/twitch-watcher"> <img alt="GitHub issues" src="https://img.shields.io/github/issues/InstreakTV/twitch-watcher"> <a href="https://asciinema.org/a/rob4Rh1EG4XFVfN4XWK67JSnf" target="_blank"><img src="https://asciinema.org/a/rob4Rh1EG4XFVfN4XWK67JSnf.svg" /></a>
</p>

## Eigenschaften
- 🎥 Richtiger HTTP Live Streaming Support (Vergiss den #4000 Fehler Code)
- 🔐 Cookie-basiertes Login
- 📜 Akzeptiert automatisch die Cookies
- 👨‍💻 Der Bot wählt automatisch einen zufälligen Streamer mit dem "drop-enabled" Tag
- 🤐 Stummgeschalteter Stream
- 🛠 Erkennen Sie ausgereifte inhaltsbasierte Streams und interagieren Sie mit ihnen 
- 🛡 Proxy Optionen
- 📽 Setzt die Auflösung des Streams automatisch auf die niedrigste Auflösung
- 🧰 Sehr anpassbare Codebase
- 📦 Bereitstellbar für VPS per Docker
- 🏳️ Hilfreiche Community
- 💬 Readme in verschiedenen Sprachen: [🇫🇷 README](https://github.com/InstreakTV/twitch-watcher/blob/languages/README_FR.md) [🇧🇷 README](https://github.com/InstreakTV/twitch-watcher/blob/languages/README_PT.md) [🇷🇺 README](https://github.com/InstreakTV/twitch-watcher/blob/languages/README_RU.md) [🇸🇰 README](https://github.com/InstreakTV/twitch-watcher/blob/languages/README_SK.md) [🇩🇪 README](https://github.com/InstreakTV/twitch-watcher/blob/languages/README_DE.md)

## Vorraussetzungen

 - Windows oder Linux OS
 - Internetverbindung (Sollte offensichtlich sein...)
 - [Nodejs](https://nodejs.org/en/download/) und [NPM](https://www.npmjs.com/get-npm)
 
## Installation
🎥 [Tutorial video von Ziyad](https://youtu.be/bwzv7wT44Ds) 🎥
### Windows
1. Logge dich in deinen Twitch Account ein
2. Öffne den Inspektor(F12 or Ctrl+Shift+I) auf der Startseite
3. Suche den gespeicherten Cookie-Bereich 
4. Kopiere **auth-token**
5. Lade die Repo runter
6. Installiere Chromium
7. Der Standardpfad lautet: C:\\Program Files (x86)\\Google\\Chrome\\Application\\chrome.exe
8. Installiere die Abhängigkeiten mit `npm install`
9. Starte das Programm mit `npm start`
### Linux
1. Logge dich in deinen Twitch Account ein
2. Öffne den Inspektor(F12 or Ctrl+Shift+I) auf der Startseite
3. Suche den gespeicherten Cookie-Bereich 
4. Kopiere **auth-token**
5. Lade die Repo runter
6. Installiere Chromium: [TUTORIAL 🤗](https://www.addictivetips.com/ubuntu-linux-tips/install-chromium-on-linux/)
7. Finde Chromium: `whereis chromium` oder `whereis chromium-browser`
8. Installiere die Abhängigkeiten mit `npm install`
9. Starte das Programm mit `npm start`

## Docker
<p align="center">
<img alt="Docker Image Version (latest by date)" src="https://img.shields.io/docker/v/d3vm/valorant-watcher"> <img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/d3vm/valorant-watcher"> <img alt="Docker Image Size (latest by date)" src="https://img.shields.io/docker/image-size/d3vm/valorant-watcher">
</p>


>Docker ist eine Reihe von PaaS-Produkten (Platform as a Service), die mithilfe der Virtualisierung auf Betriebssystemebene Software in Paketen bereitstellen, die als Container bezeichnet werden. Container sind voneinander isoliert und bündeln ihre eigene Software, Bibliotheken und Konfigurationsdateien. Alle Container werden von einem einzelnen Betriebssystemkern ausgeführt und verbrauchen daher weniger Ressourcen als virtuelle Maschinen. 
### Vorraussetzungen
- [Docker](https://docs.docker.com/get-docker/)
- [Docker-Compose](https://docs.docker.com/compose/install/)

### Verwendung
1. Downloade docker-compose-example.yml
2. Nenne die Datei docker-compose.yml
3. Öffne und ersetze den **token** Umgebungsdatensatz
4. Führen Sie den Befehl `docker-compose up -d` aus
## Abhängigkeiten
<p align="center">
<img alt="GitHub package.json dependency version (subfolder of monorepo)" src="https://img.shields.io/github/package-json/dependency-version/InstreakTV/twitch-watcher/puppeteer-core"> <img alt="GitHub package.json dependency version (subfolder of monorepo)" src="https://img.shields.io/github/package-json/dependency-version/InstreakTV/twitch-watcher/cheerio"> <img alt="GitHub package.json dependency version (subfolder of monorepo)" src="https://img.shields.io/github/package-json/dependency-version/InstreakTV/twitch-watcher/inquirer"> <img alt="GitHub package.json dependency version (subfolder of monorepo)" src="https://img.shields.io/github/package-json/dependency-version/InstreakTV/twitch-watcher/dotenv"> <img alt="GitHub package.json dependency version (subfolder of monorepo)" src="https://img.shields.io/github/package-json/dependency-version/InstreakTV/twitch-watcher/dayjs"> <img alt="GitHub package.json dependency version (prod)" src="https://img.shields.io/github/package-json/dependency-version/InstreakTV/twitch-watcher/tree-kill">
</p>

## Problembehandlung

### Wie sieht der Token aus?
auth-token: `rxk38rh5qtyw95fkvm7kgfceh4mh6u`
___


### Streamers.json ist leer?

Versuche es mit einem höheren Delay.
Normales delay:
```javascript
const scrollDelay = 2000;
```
[Gehe zum Code](https://github.com/InstreakTV/twitch-watcher/blob/12dce8065423861971b7088563ad936b2dcc2559/app.js#L15)
___
### Etwas ist schiefgelaufen?
Probiere den non-headless mode aus. Setze den Wert auf `true`, wie hier im Beispiel:
```javascript
const showBrowser = true;
```
[Gehe zum Code](https://github.com/InstreakTV/twitch-watcher/blob/12dce8065423861971b7088563ad936b2dcc2559/app.js#L15)
___
### Proxy?

Natürlich:
```javascript
const proxy = ""; // "ip:port" By https://github.com/Jan710
```
[Gehe zum Code](https://github.com/InstreakTV/twitch-watcher/blob/12dce8065423861971b7088563ad936b2dcc2559/app.js#L15)  

ODER
Mit Docker:
```
proxy=PROXY_IP_ADDRESS:PROXY_PORT
```
___
### Screenshot ohne non-headless mode
```javascript
const browserScreenshot = false;
```
[Gehe zum Code](https://github.com/InstreakTV/twitch-watcher/blob/12dce8065423861971b7088563ad936b2dcc2559/app.js#L15)

## Spenden
Bitte spende um das Projekt am Leben zu erhalten!

Insbesondere die Drop-farmer, die viel Geld mit dem Programm verdienen!🤓  

<a href="https://www.buymeacoffee.com/D3v" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>


## Support
 - Twitter Link: [https://twitter.com/InstreakTV](https://twitter.com/InstreakTV)
 - Discord Link: [https://discord.gg/s8AH4aZ](https://discord.gg/s8AH4aZ) (Old Server please dm K.K. Slider#0815)

## Haftungsausschluss
Dieser Code dient ausschließlich Bildungs- und Forschungszwecken.
Versuchen Sie nicht, mit den hier enthaltenen Informationen gegen das Gesetz zu verstoßen.
Ich bin nicht verantwortlich für illegale Handlungen.
Vervielfältigung und Vervielfältigung sind gestattet, sofern die Quelle angegeben ist. 
