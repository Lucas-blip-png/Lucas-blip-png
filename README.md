<h1 align="center">Lucas Daniel Duarte Cabral</h1>

<p align="center">
  <b>Back-end Developer · Java 21 · Spring Boot · PostgreSQL · RabbitMQ · Docker</b><br />
  Systems Analysis and Development student at UCDB · Campo Grande, MS, Brazil (UTC−4)<br />
  Open to back-end internships and junior developer roles — on-site, remote or international
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/lucasdanielcabral"><img alt="LinkedIn: lucasdanielcabral" src="https://img.shields.io/badge/LinkedIn-lucasdanielcabral-0A66C2?style=flat-square" /></a>
  <a href="mailto:lucasdanielfaculdade@gmail.com"><img alt="Email: lucasdanielfaculdade@gmail.com" src="https://img.shields.io/badge/Email-lucasdanielfaculdade%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" /></a>
</p>

---

## About me

I build back-end services with **Java 21 and Spring Boot**, and I focus on what keeps software correct under load: **automated tests against real infrastructure, concurrency control, asynchronous messaging and containerized delivery**.

- **Recently shipped:** closed 6 IDOR (broken access control) issues and added Testcontainers integration tests, Swagger/OpenAPI and Flyway migrations to [ASUS RPG Platform](https://github.com/Lucas-blip-png/Asus-site)
- **Building:** [Mesa Pronta](https://github.com/Lucas-blip-png/mesa-pronta), a Discord bot with RabbitMQ reminders
- **Learning:** Kafka, cloud deployment and observability
- **Education:** Systems Analysis and Development, Universidade Católica Dom Bosco (UCDB), 2024 – 2027
- **Languages:** Portuguese (native) · English (B1, intermediate)

## Featured projects

### [ASUS RPG Platform](https://github.com/Lucas-blip-png/Asus-site) — full-stack virtual tabletop

My main project: 160+ commits, continuous deployment on Railway.

- Spring Boot REST API + **WebSocket (STOMP)** for real-time play; **JWT** auth with Spring Security and role-based campaign permissions (owner, game master, player)
- **Security:** audited the API and fixed 6 IDOR vulnerabilities so users can only reach their own resources
- **Quality:** unit tests (JUnit 5, Mockito), MockMvc API flows and an integration test on **real PostgreSQL 17 via Testcontainers**; suite grew from 22 to 38 tests; Swagger/OpenAPI docs with JWT Bearer
- **Schema safety:** replaced Hibernate `ddl-auto=update` with **Flyway** (V1 baseline of the 39-table schema, `validate` in production)
- **LGPD** features (data export, consent, anonymization), audit history and snapshots; React SPA bundled into a single Docker image

`Java 21` `Spring Boot` `Spring Security` `JPA` `WebSocket` `React` `PostgreSQL` `Flyway` `Docker`

### [Discord Lyrics Status](https://github.com/Lucas-blip-png/Discord-Lyrics-Status) — desktop app that syncs song lyrics to Discord

- Detects the song playing on the PC, fetches synced lyrics and updates the Discord status line by line, with a configurable rate limit
- All-in-one `.exe` with tray icon and autostart, **12 UI languages** (i18n), Spotify API and Android versions
- CI on **GitHub Actions** to build the `.exe`

`Python` `Discord API` `Spotify API` `GitHub Actions`

### [Mesa Pronta](https://github.com/Lucas-blip-png/mesa-pronta) — Discord bot for scheduling tabletop RPG sessions

- **No double booking:** joining locks the session row with `SELECT ... FOR UPDATE` plus a `UNIQUE` constraint; a test fires **20 concurrent joins at 1 seat** and asserts exactly one succeeds
- **Reliable reminders:** a scheduler polls due sessions with `FOR UPDATE SKIP LOCKED` and publishes 24h/1h reminders to **RabbitMQ**; the consumer retries 3× with backoff, then parks failures in a **dead-letter queue**
- Integration tests with **Testcontainers**, Docker Compose and CI on GitHub Actions

`Java 21` `Spring Boot` `JDA` `PostgreSQL` `RabbitMQ` `Testcontainers` `Docker`

### [Radar de Vagas](https://github.com/Lucas-blip-png/radar-vagas) — job radar and application tracker

- Scheduled collection from public job APIs (GitHub Issues, Remotive), with filtering, scoring and URL deduplication
- Application pipeline with follow-up dates and a REST API; deliberately does not auto-apply, to respect each site's terms of service
- API clients tested against recorded JSON with `MockRestServiceServer`, so CI never depends on the network

`Java 21` `Spring Boot` `Flyway` `Docker` `GitHub Actions`

### [SteamQuest](https://github.com/HeFidelis/trabalho-bd2) — digital-game e-commerce in PostgreSQL (UCDB team project)

- Implemented the `fn_finalizar_pedido` transaction: order locking with `SELECT ... FOR UPDATE`, status validation, payment creation and order finalization

`PostgreSQL` `PL/pgSQL` `Git`

## Tech stack

**Back-end**<br>
![Java 21](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![OpenAPI](https://img.shields.io/badge/OpenAPI-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white)

**Data & messaging**<br>
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white)

**Testing & delivery**<br>
![JUnit 5](https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white)
![Testcontainers](https://img.shields.io/badge/Testcontainers-291A3F?style=flat-square&logo=testcontainers&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Front-end**<br>
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**Also used:** Spring Data JPA · JDA · Mockito · MockMvc · SQL / PL/pgSQL · H2 · Vite · Git · Railway · Discord API · Spotify API

## GitHub activity

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/main/profile-3d-contrib/profile-night-green.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/main/profile-3d-contrib/profile-green-animate.svg" />
    <img alt="3D contribution graph of Lucas-blip-png" src="https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/main/profile-3d-contrib/profile-green-animate.svg" />
  </picture>
</p>

## Development stats

<!--START_SECTION:waka-->
![Code Time](http://img.shields.io/badge/Code%20Time-0%20secs-blue?style=flat)

![Profile Views](http://img.shields.io/badge/Profile%20Views-37-blue?style=flat)

**🐱 My GitHub Data** 

> 📦 153.1 kB Used in GitHub's Storage 
 > 
> 🏆 528 Contributions in the Year 2026
 > 
> 🚫 Not Opted to Hire
 > 
> 📜 14 Public Repositories 
 > 
> 🔑 1 Private Repositories 
 > 
**I'm a Night 🦉** 

```text
🌞 Morning                133 commits         ███░░░░░░░░░░░░░░░░░░░░░░   10.32 % 
🌆 Daytime                199 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.44 % 
🌃 Evening                735 commits         ██████████████░░░░░░░░░░░   57.02 % 
🌙 Night                  222 commits         ████░░░░░░░░░░░░░░░░░░░░░   17.22 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   131 commits         ███░░░░░░░░░░░░░░░░░░░░░░   10.16 % 
Tuesday                  96 commits          ██░░░░░░░░░░░░░░░░░░░░░░░   07.45 % 
Wednesday                162 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.57 % 
Thursday                 108 commits         ██░░░░░░░░░░░░░░░░░░░░░░░   08.38 % 
Friday                   75 commits          █░░░░░░░░░░░░░░░░░░░░░░░░   05.82 % 
Saturday                 277 commits         █████░░░░░░░░░░░░░░░░░░░░   21.49 % 
Sunday                   440 commits         █████████░░░░░░░░░░░░░░░░   34.13 % 
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
Python                   5 repos             ██████████░░░░░░░░░░░░░░░   38.46 % 
C++                      4 repos             ████████░░░░░░░░░░░░░░░░░   30.77 % 
Java                     3 repos             ██████░░░░░░░░░░░░░░░░░░░   23.08 % 
PLpgSQL                  1 repo              ██░░░░░░░░░░░░░░░░░░░░░░░   07.69 % 
```



**Timeline**

![Lines of Code chart](https://raw.githubusercontent.com/Lucas-blip-png/Lucas-blip-png/main/assets/bar_graph.png)


 Last Updated on 29/10/2026 13:37:24 UTC
<!--END_SECTION:waka-->

---

<p align="center">
  Open to back-end internships and junior developer roles · <a href="https://www.linkedin.com/in/lucasdanielcabral">LinkedIn</a> · <a href="mailto:lucasdanielfaculdade@gmail.com">lucasdanielfaculdade@gmail.com</a>
</p>
