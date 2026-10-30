<div align="center">
  <img src="./header.svg" alt="The Safii Gazette — Developer ships, learns, ships again" width="100%" />
</div>

<p align="center">
  <a href="https://linkedin.com/in/muhamad-safii-eko-kuncoro-b8053731b"><img src="https://img.shields.io/badge/LinkedIn-Muhamad_Safii-1a1a1a?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:firelord@gmail.com"><img src="https://img.shields.io/badge/Email-firelord@gmail.com-b3261e?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Status-Open_to_work-8a6d3b?style=flat-square" alt="Open to work" />
</p>

---

## 🗞️ THE STORY

**TANGERANG** — A web developer with an Information Systems background keeps building, breaking, and rebuilding things a little better each time. He works across Laravel and React, with a soft spot for the backend: APIs, databases, and the plumbing that keeps an app honest.

His thesis, a retrieval-augmented chatbot for a hospital website, taught him that shipping is only half the job: measuring, learning, and improving is the other half. His motto is printed in small type at the bottom of every page: *clean code beats clever code.*

| AT A GLANCE | |
|---|---|
| **Name** | Muhamad Safii |
| **Occupation** | Junior Web Developer (backend-leaning, fullstack-capable) |
| **Education** | B.Sc. Information Systems, Universitas Gunadarma, Class of 2026 |
| **Dateline** | Tangerang, Indonesia |
| **Known for** | Laravel · REST APIs · RAG chatbots |

---

## 📰 TOP STORY: A CHATBOT THAT ANSWERS FOR A HOSPITAL

*RSU Aulia's website now answers visitor questions from its own information, using Retrieval-Augmented Generation. The system is split into small services, each with one job.*

```mermaid
flowchart LR
    U([👤 Visitor]) --> N["Next.js<br/>(Vercel)"]
    N -- "question" --> F
    F -- "grounded answer" --> N
    N <-- "login & history" --> L

    subgraph VPS ["VPS · Docker Compose + Nginx"]
        F["FastAPI<br/>RAG engine"]
        L["Laravel<br/>auth & conversations"]
        M[("MySQL")]
        L --> M
    end

    F --> V[("Astra DB<br/>vectors")]
    F --> G["Gemini<br/>LLM + embeddings"]
```

<details>
<summary><b>Continued on page 2: why it was built this way</b></summary>

<br/>

- **FastAPI** owns the RAG pipeline (LangChain, retrieval, generation) and has no direct MySQL connection.
- **Laravel** owns authentication and conversation history, keeping business data in MySQL.
- **Next.js** talks directly to FastAPI for answers, so the chat stays fast.
- **RAGAS** measured answer quality across six metrics, using 20 evaluation scenarios.

</details>

---

## 📌 WANTED

> ### WANTED: A TEAM TO BUILD WITH
> **Position:** Junior Web Developer (backend or fullstack)
> **Experience:** Thesis defended, side projects shipped, always iterating
> **Offers:** Curiosity, discipline with Git, and a habit of reading the docs and asking good questions
> **Seeks:** A team of experienced engineers to learn from
>
> **Apply within:** [LinkedIn](https://linkedin.com/in/muhamad-safii-eko-kuncoro-b8053731b) · [Email](mailto:firelord@gmail.com)

---

## 🗂️ CLASSIFIEDS: SKILLS FOR HIRE

| Section | Listings |
|---|---|
| **Backend** | PHP 8 · Laravel 11 · FastAPI · REST API · JWT |
| **Frontend** | JavaScript (ES6+) · React.js · Next.js · Tailwind CSS · Bootstrap 5 |
| **Database** | MySQL · Astra DB (vector) |
| **AI** | LangChain · Gemini · RAGAS |
| **Tooling** | Git · GitHub · Docker Compose · Nginx · Postman · VS Code |

---

## 🌦️ FORECAST

**Partly cloudy with a high chance of microservices.**
Learning this season: **Go**, **REST API security**, and **cloud microservices**.
Currently building: **[Jelajah Tangerang](https://github.com/ekodee)**, a local tourism and culinary discovery platform.

---

## 📈 MARKET REPORT: CONTRIBUTION ACTIVITY

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ekodee/ekodee/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ekodee/ekodee/output/github-snake.svg" />
    <img alt="Contribution snake" src="https://raw.githubusercontent.com/ekodee/ekodee/output/github-snake.svg" />
  </picture>
</div>

---

## ✉️ LETTERS TO THE EDITOR

Hiring, mentoring, or just want to talk Laravel, APIs, or RAG? Write in.

<p align="center">
  <a href="https://linkedin.com/in/muhamad-safii-eko-kuncoro-b8053731b"><b>LinkedIn</b></a> ·
  <a href="mailto:firelord@gmail.com"><b>Email</b></a> ·
  <a href="https://github.com/ekodee"><b>GitHub</b></a>
</p>

---

<p align="center"><sub><b>EDITOR’S NOTE:</b> this edition is a work in progress. Updates will be printed as the editor learns more.</sub></p>
