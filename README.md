## Hello! I'm Rita 👋 😺

Full-stack engineer building production software across API, web and mobile: **TypeScript / NestJS** services on **PostgreSQL** with **React** and **React Native** clients, plus two **Ruby on Rails 8** apps of my own in daily production use. I came to software after a decade of process and R&D engineering, doing root-cause work on noisy real-world data.

📍 Taiwan · Remote · Available 13:00–23:00 GMT+8 (most of the EU workday, US East Coast mornings) · Open to full-time or contract

🌐 <a href="https://yuhruh.github.io" target="_blank">Portfolio</a> · 📄 <a href="https://drive.google.com/file/d/1DLhEfZ1f2Id39poz2CLL_M3grFCd_5np/view?usp=drive_link" target="_blank">Resume</a> · 💼 <a href="https://www.linkedin.com/in/yuruhuang/" target="_blank">LinkedIn</a>

![Profile views](https://komarev.com/ghpvc/?username=yuhruh&color=green&style=flat-square)

## 💼 Now

**Full-Stack Builder**, early-stage US startup (independent contractor, remote), since 2026.07. I work on a production app on web, iOS and Android (TypeScript, NestJS, PostgreSQL, React, React Native):

- **API and data model:** NestJS REST endpoints and PostgreSQL schema changes; merged business rules that had drifted apart across clients into one server-side resolver, so API, web and mobile enforce the same rules.
- **Type-safe contracts:** a TypeScript code-generation pipeline that emits Swift and Kotlin from one schema.
- **Integration reliability:** per-device push delivery receipts; webhook and inbound-email handlers that fail loudly instead of reporting success while dropping data.
- **AI-assisted, human-owned delivery:** a Claude Code pipeline where each ticket runs in its own git worktree, with a root-cause plan I approve, tests on all platforms and a reviewed PR.

## 🚀 Projects

### 🏠 Household Tracker · shared bill and household-supplies tracker PWA in zh-TW and English
Replaced my family's Google Sheet. Rails 8.1 · PostgreSQL · Hotwire · Web Push · Gmail API · Google Drive API · Solid Queue · Apache ECharts · Sentry · Railway

- **Sheet to product:** shared ledgers, one-step bill entry by scanning a Taiwan bill's barcodes (or reading a bill PDF or photo), recurring bills that never duplicate, and a preview-then-commit CSV import that is safe to re-run.
- **Bills that fill themselves in:** a daily job syncs gas bills from the utility's site; electricity and water bills arrive as forwarded e-bill emails, read through the Gmail API only when the company signed them. Each bill is matched to its period, never added twice, and marked paid when the company says so.
- **Supplies and run-out forecasts:** household stock from product barcodes, Taiwan e-invoice QR codes and invoice PDFs, with each item's usage rate, run-out date and a restock alert in time to buy more.
- **Reliable reminders:** one daily digest per member in their own time zone, by Web Push, email and in-app inbox. Unique indexes act as locks so a double run never sends twice.
- **Operations and testing:** encrypted weekly database backups plus a Google Drive backup; about 730 Minitest tests with Brakeman, RuboCop and dependency audits in CI; security-scan findings fixed as they come in.

<a href="https://github.com/yuhruh/HouseHold_Notification" target="_blank">Code</a> · <a href="https://github.com/yuhruh/HouseHold_Notification/tree/main/docs/adr" target="_blank">Design decisions (6 ADRs)</a> · <a href="https://household-tracker.up.railway.app" target="_blank">Live app (invite-only)</a>

### 🐈 Pet Tracker · pet-care app for households, on web, PWA and Android, in English, 繁體中文 and 日本語
Rails 8.1 · PostgreSQL · Hotwire · Hotwire Native (Kotlin) · Firebase Cloud Messaging · Solid Queue · Nokogiri · Gemini · Railway

- **Price scraping:** a monthly Nokogiri scraper across two Taiwan shopping sites (BigGo HTML, PChome JSON API), ranked by NT$ per kg. Selectors survive hashed class names; a changed layout raises an alert instead of passing as "no results"; rate-limited, follows robots.txt, tested against saved HTML fixtures.
- **Collaboration:** owners invite caregivers and share read-only links, with one role policy behind every permission; care logs update live via Turbo Streams.
- **Background work and AI:** care and weight reminders at each household's local time with fallback from Android push (Firebase) to LINE to email, plus daily Google Drive backups; Gemini vision turns health-checkup photos into validated ActiveRecord records.
- **Testing:** about 700 Minitest tests (61 browser tests) with Brakeman, RuboCop and dependency audits in CI.

<a href="https://github.com/yuhruh/Pet_Feeding_Tracker_v4" target="_blank">Code</a> · <a href="https://github.com/yuhruh/Pet_Feeding_Tracker_v4/blob/main/ARCHITECTURE.md" target="_blank">Architecture</a> · <a href="https://pet-feeding-tracker-v4.up.railway.app" target="_blank">Live app (invite-only)</a>

## 🌱 Open Source

- **SerpApi client libraries:** <a href="https://github.com/serpapi/serpapi-ruby/pull/48" target="_blank">serpapi-ruby #48</a> (merged): corrected the README's async section, since `search_archive` does not block. Docs fixes open in <a href="https://github.com/serpapi/serpapi-javascript/pull/61" target="_blank">serpapi-javascript #61</a> and <a href="https://github.com/serpapi/serpapi-cpp/pull/8" target="_blank">serpapi-cpp #8</a>.
- **GitNexus:** <a href="https://github.com/abhigyanpatwari/GitNexus/pull/4152" target="_blank">#4152</a> (open): restore web chat history across page reloads. <a href="https://github.com/abhigyanpatwari/GitNexus/pull/4147" target="_blank">#4147</a> (open): replace scattered `console.log` calls with a dev-only debug logger.
- **Rails:** <a href="https://github.com/rails/rails/pull/58866" target="_blank">rails/rails #58866</a> (open): fix for extended deterministic queries on encrypted attributes that also use `normalizes`. <a href="https://github.com/svenfuchs/rails-i18n/pull/1171" target="_blank">rails-i18n #1171</a> (merged): missing zh-TW keys and translations.

## 🛠️ Skill Set

| Category | Skills |
| --- | --- |
| **Languages** | ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=fff&style=flat) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=000&style=flat) ![Ruby](https://img.shields.io/badge/Ruby-CC342D?logo=ruby&logoColor=fff&style=flat) ![SQL](https://img.shields.io/badge/SQL-336791?logo=postgresql&logoColor=fff&style=flat) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=fff&style=flat) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=fff&style=flat) |
| **Backend** | ![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=fff&style=flat) ![Node.js](https://img.shields.io/badge/Node.js-5FA04E?logo=nodedotjs&logoColor=fff&style=flat) ![Ruby on Rails](https://img.shields.io/badge/Ruby%20on%20Rails%208-CC0000?logo=rubyonrails&logoColor=fff&style=flat) ![Solid Queue](https://img.shields.io/badge/Solid%20Queue-555?style=flat) ![REST](https://img.shields.io/badge/REST%20APIs-555?style=flat) ![OAuth](https://img.shields.io/badge/OAuth-EB5424?logo=auth0&logoColor=fff&style=flat) ![Google APIs](https://img.shields.io/badge/Gmail%20%2F%20Drive%20APIs-4285F4?logo=google&logoColor=fff&style=flat) ![Nokogiri](https://img.shields.io/badge/Nokogiri-555?style=flat) |
| **Frontend & Mobile** | ![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=000&style=flat) ![React Native](https://img.shields.io/badge/React%20Native-20232A?logo=react&logoColor=61DAFB&style=flat) ![Hotwire](https://img.shields.io/badge/Hotwire-FFE801?logo=hotwire&logoColor=000&style=flat) ![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?logo=tailwindcss&logoColor=fff&style=flat) ![PWA](https://img.shields.io/badge/PWA%20%2F%20Web%20Push-5A0FC8?logo=pwa&logoColor=fff&style=flat) ![ECharts](https://img.shields.io/badge/Apache%20ECharts-AA344D?logo=apacheecharts&logoColor=fff&style=flat) |
| **Data, Infra & Quality** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=fff&style=flat) ![Railway](https://img.shields.io/badge/Railway-131313?logo=railway&logoColor=fff&style=flat) ![Render](https://img.shields.io/badge/Render-46E3B7?logo=render&logoColor=000&style=flat) ![Heroku](https://img.shields.io/badge/Heroku-430098?logo=heroku&logoColor=fff&style=flat) ![Sentry](https://img.shields.io/badge/Sentry-362D59?logo=sentry&logoColor=fff&style=flat) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=fff&style=flat) ![Minitest](https://img.shields.io/badge/Minitest-CC342D?style=flat) ![Brakeman](https://img.shields.io/badge/Brakeman-555?style=flat) ![RuboCop](https://img.shields.io/badge/RuboCop-000?logo=rubocop&logoColor=fff&style=flat) ![Firebase Cloud Messaging](https://img.shields.io/badge/Firebase%20Cloud%20Messaging-DD2C00?logo=firebase&logoColor=fff&style=flat) |
| **AI** | ![Gemini](https://img.shields.io/badge/Gemini%20vision%20API-8E75B2?logo=googlegemini&logoColor=fff&style=flat) ![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?logo=claude&logoColor=fff&style=flat) |

## 🧭 Before software

- **Career transition (2023.05 – 2026.06):** completed Launch School's mastery-based software engineering program and built the two apps above.
- **Isola Group, Global Process Engineer (2018–2023):** led international product development across R&D, production and customer teams; solved raw-material and process bottlenecks through root-cause analysis.
- **Nan Ya Plastics, R&D → QA → Technical Support Engineer (2013–2017):** copper-foil quality project with +$3.0M/month revenue; a new measurement method that cut deviation 60%; 10 patent specifications across Asia-Pacific.
- **Education:** M.S. Chemistry, National Taiwan University · B.S. Chemistry, National Tsing Hua University

## 😎 Fun Facts
In my downtime, I love researching cat 😼 behavior, doing core exercises 💪, and practicing yoga.

## 📫 Reach out and connect with me

- <a href="https://yuhruh.github.io" target="_blank">Portfolio</a>
- <a href="https://www.linkedin.com/in/yuruhuang/" target="_blank">LinkedIn</a>
- <a href="mailto:yuhruhgrape@gmail.com">Email</a>

![GitHub stats](https://github-readme-stats.vercel.app/api?username=yuhruh&show_icons=true&theme=dark&commits_year=2026)
