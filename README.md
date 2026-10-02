<h1 align="center">Hi, I'm Lucas 👋</h1>

<p align="center">
  <b>Back-end Developer · Java & Spring Boot</b><br>
  Systems Analysis and Development student · Brazil 🇧🇷
</p>

---

I build back-end systems with **Java 21 and Spring Boot**, and I care about the parts that make software hold up in production: **automated tests, concurrency, messaging and containers**.

- 🎲 Currently building **[Mesa Pronta](https://github.com/Lucas-blip-png/mesa-pronta)**, a Discord bot that schedules tabletop RPG sessions with RabbitMQ reminders
- 🧱 Maintaining **[ASUS RPG Platform](https://github.com/Lucas-blip-png/Asus-site)**, a full-stack virtual tabletop (Spring Boot + React)
- 📚 Learning: Kafka, cloud deployment and observability
- 🇧🇷 Português nativo · 🇺🇸 English for technical reading and writing

## 🛠️ Tech stack

**Back-end**<br>
![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

**Data & messaging**<br>
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white)

**Testing & DevOps**<br>
![JUnit5](https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white)
![Testcontainers](https://img.shields.io/badge/Testcontainers-291A3F?style=flat-square&logo=testcontainers&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Front-end**<br>
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)

## 🚀 Featured projects

### [🎲 Mesa Pronta](https://github.com/Lucas-blip-png/mesa-pronta)
Discord bot for scheduling tabletop RPG sessions.
- Session booking with attendance buttons; the last seat is protected by `SELECT ... FOR UPDATE`, proven by a test where **20 threads race for 1 seat**
- 24h and 1h reminders through **RabbitMQ**, with retry and a **dead-letter queue**
- Integration tests with **Testcontainers** (real PostgreSQL and RabbitMQ), Docker Compose and CI on GitHub Actions

`Java 21` `Spring Boot` `JDA` `PostgreSQL` `RabbitMQ` `Testcontainers` `Docker`

### [🧱 ASUS RPG Platform](https://github.com/Lucas-blip-png/Asus-site)
Full-stack SaaS virtual tabletop for the ASUS RPG system.
- REST API + **WebSocket (STOMP)** for real-time play, **JWT** auth with Spring Security, rate limiting and CORS
- Automated character sheets, campaigns and permissions, dice rolls, audit history and snapshots
- **LGPD** features (data export, consent, anonymization), marketplace, OBS overlay
- Single-service Docker deploy on Railway (React bundled into Spring Boot)

`Java 21` `Spring Boot` `Spring Security` `JPA` `WebSocket` `React` `PostgreSQL`

### [🎵 Discord Lyrics Status](https://github.com/Lucas-blip-png/Discord-Lyrics-Status)
Desktop tool that syncs the lyrics of the song you're playing to your Discord status, line by line.
- Detects the song playing on the PC, fetches synced lyrics and updates the status with a configurable rate limit
- Packaged `.exe` with an all-in-one menu, tray icon, autostart and **12 UI languages**; Spotify API and Android versions

`Python` `Windows` `Android`

## 📈 GitHub activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/output/github-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/output/github-snake.svg">
  <img alt="Snake eating my contribution graph" src="https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/output/github-snake.svg">
</picture>
