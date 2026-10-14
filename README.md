<h1 align="center">Hi, I'm Lucas 👋</h1>

<p align="center">
  <b>Back-end Developer · Java & Spring Boot</b><br>
  Systems Analysis and Development student at UCDB · Campo Grande, MS, Brazil 🇧🇷<br><br>
  <a href="mailto:lucasdanielfaculdade@gmail.com"><img src="https://img.shields.io/badge/Email-lucasdanielfaculdade%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

I build back-end systems with **Java 21 and Spring Boot**, and I care about the parts that make software hold up in production: **automated tests, concurrency, messaging and containers**.

- 🎲 Currently building **[Mesa Pronta](https://github.com/Lucas-blip-png/mesa-pronta)**, a Discord bot that schedules tabletop RPG sessions with RabbitMQ reminders
- 🧱 Maintaining **[ASUS RPG Platform](https://github.com/Lucas-blip-png/Asus-site)**, a full-stack virtual tabletop (Spring Boot + React)
- 📚 Learning: Kafka, cloud deployment and observability
- 🎯 Open to back-end internship and junior developer roles
- 🇧🇷 Native Portuguese · 🇺🇸 Intermediate English (B1)

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

**Languages & more**<br>
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![OpenAPI](https://img.shields.io/badge/OpenAPI-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white)
![Mockito](https://img.shields.io/badge/Mockito-78A641?style=flat-square)
![Discord API](https://img.shields.io/badge/Discord_API-5865F2?style=flat-square&logo=discord&logoColor=white)
![Spotify API](https://img.shields.io/badge/Spotify_API-1DB954?style=flat-square&logo=spotify&logoColor=white)

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
### [🎮 SteamQuest](https://github.com/HeFidelis/trabalho-bd2)
E-commerce of digital games modeled in PostgreSQL, built as an academic team project at UCDB.
- Owned the `fn_finalizar_pedido` transaction: order locking (`SELECT ... FOR UPDATE`), concurrent key reservation (`SKIP LOCKED`), status validation and payment generation.
- Versioned with Git and developed collaboratively.

`PostgreSQL` `SQL` `Git`

## 📈 GitHub activity

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/main/profile-3d-contrib/profile-night-green.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/main/profile-3d-contrib/profile-green-animate.svg" />
    <img alt="Gráfico 3D de contribuições de Lucas-blip-png" src="https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/main/profile-3d-contrib/profile-green-animate.svg" />
  </picture>
</p>

## 📊 Development stats

<!--START_SECTION:waka-->
![Profile Views](http://img.shields.io/badge/Profile%20Views-0-blue?style=flat)

**🐱 My GitHub Data** 

> 📦 152.9 kB Used in GitHub's Storage 
 > 
> 🏆 467 Contributions in the Year 2026
 > 
> 🚫 Not Opted to Hire
 > 
> 📜 13 Public Repositories 
 > 
> 🔑 1 Private Repositories 
 > 
**I'm a Night 🦉** 

```text
🌞 Morning                132 commits         ███░░░░░░░░░░░░░░░░░░░░░░   10.44 % 
🌆 Daytime                195 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.43 % 
🌃 Evening                718 commits         ██████████████░░░░░░░░░░░   56.80 % 
🌙 Night                  219 commits         ████░░░░░░░░░░░░░░░░░░░░░   17.33 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   119 commits         ██░░░░░░░░░░░░░░░░░░░░░░░   09.41 % 
Tuesday                  95 commits          ██░░░░░░░░░░░░░░░░░░░░░░░   07.52 % 
Wednesday                157 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.42 % 
Thursday                 106 commits         ██░░░░░░░░░░░░░░░░░░░░░░░   08.39 % 
Friday                   75 commits          █░░░░░░░░░░░░░░░░░░░░░░░░   05.93 % 
Saturday                 272 commits         █████░░░░░░░░░░░░░░░░░░░░   21.52 % 
Sunday                   440 commits         █████████░░░░░░░░░░░░░░░░   34.81 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: America/Cuiaba

💬 Programming Languages: 
No Activity Tracked This Week

🔥 Editors: 
No Activity Tracked This Week

🐱‍💻 Projects: 
No Activity Tracked This Week

💻 Operating System: 
No Activity Tracked This Week
```

🤖 **AI Coding This Week** 

```text
No AI Coding Activity Tracked This Week
```

**I Mostly Code in Python** 

```text
Python                   5 repos             ██████████░░░░░░░░░░░░░░░   41.67 % 
C++                      3 repos             ██████░░░░░░░░░░░░░░░░░░░   25.00 % 
Java                     3 repos             ██████░░░░░░░░░░░░░░░░░░░   25.00 % 
PLpgSQL                  1 repo              ██░░░░░░░░░░░░░░░░░░░░░░░   08.33 % 
```



**Timeline**

![Lines of Code chart](https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/main/assets/bar_graph.png)


 Last Updated on 14/10/2026 12:17:47 UTC
<!--END_SECTION:waka-->
