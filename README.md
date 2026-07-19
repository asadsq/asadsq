# Hi, I'm Asad 👋

Lead engineer with **12+ years** building enterprise software that runs on the cloud. Most of my day job is deep in Java, AWS, and distributed systems — lately with a focus on **LLM integration** into production pipelines. Off the clock, I build developer tools and small apps, usually pairing spec-driven, agent-augmented workflows with real engineering rigor: tests, code review, CI, and verification gates.

- 🔭 Currently: Lead Engineer at CorroHealth, working on LLM-driven medical-coding accuracy and real-time anomaly detection at fleet scale (1,500+ nodes).
- 🧰 For fun: MCP servers, IntelliJ plugins, and SwiftUI apps — the pinned repos below.
- 🎓 B.S. Computer Science, University of Michigan, Ann Arbor — Forever a Wolverine &nbsp;![Go Blue](https://img.shields.io/badge/〽️_Michigan-Go_Blue!-FFCB05?style=flat-square&labelColor=00274C)
- 📫 Reach me: asadsq@umich.edu

### Tech I work with every day

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Rundeck](https://img.shields.io/badge/Rundeck-F73F39?style=flat-square)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Dynatrace](https://img.shields.io/badge/Dynatrace-1496FF?style=flat-square&logo=dynatrace&logoColor=white)
![PagerDuty](https://img.shields.io/badge/PagerDuty-06AC38?style=flat-square&logo=pagerduty&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white)

`Java` · `AWS (SDK, EC2, S3, SQS, Lambda)` · `REST APIs` · `LLM integration` · `Gradle / Maven` · `GitHub` · `Rundeck · Jenkins` · `Linux` · `Dynatrace · Loggly · PagerDuty` · `Claude Code`

### Tech I've explored

![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

`Swift / SwiftUI` · `Kotlin` · `Spring Boot` · `JavaScript / TypeScript` · `HTML / CSS` · `React · Node.js · Express · Angular` · `MongoDB` · `Docker` · `Model Context Protocol` · `IntelliJ Platform SDK`

---

## Featured projects

### 🗺️ [Cartograph](https://github.com/asadsq/cartograph-mcp-server) — MCP server for AI-agent codebase review
`Java 21` · `Maven` · `Model Context Protocol SDK 2.0` · `JUnit 5` · `GitHub Actions`

A Model Context Protocol server that gives AI coding agents a complete, queryable map of a codebase's dependency and call graph — exhaustive, deterministic answers to whole-graph questions that agents can't reliably reconstruct by grep-and-read alone.

Think of it as an `init` for your coding agent — but on steroids: rather than a one-time summary of your project, it plugs into an agent you already use as a live tool it can query on demand, so its understanding of your codebase stays exact instead of going stale.

💙 **My favorite project at the moment** — and the one I'm most ambitiously building on right now.

- Complete **blast-radius** analysis (full transitive closure of dependents, grouped by distance), circular-dependency detection, in-degree "hotspot" ranking, and shortest dependency path between modules.
- Every tool explains what it did in plain English, with honest resolved-vs-unresolved coverage reporting — trust over false precision.
- **Privacy-first, local-only** deployment: runs entirely on your machine, so proprietary source never leaves it.
- Ships as a shaded, runnable JAR with JUnit 5 tests, MCP Inspector verification, and GitHub Actions CI.

### ✅ [jb-todo-enhancer](https://github.com/asadsq/jb-todo-enhancer) — IntelliJ IDEA plugin
`Kotlin` · `IntelliJ Platform Gradle Plugin 2.x` · `IDEA 2025.2` · `JUnit 5` · `GitHub Actions`

Upgrades IntelliJ's built-in TODO handling. Scoped in plan mode as a weekly MVP, with 13 unit tests, CI, and Plugin Verifier compatibility across four IDE builds (2025.2–2026.2).

🎤 *Why I built it: to have something worth presenting at a JetBrains developer conference. I've submitted a speaker proposal and am hoping to share this work with the wider plugin community — a bit of building out loud beyond the day job.*

- Structured TODO syntax — `// TODO(@asad) !p1 #backend due:2026-07-10` — parsing assignee, priority, tags, and due date (plain `// TODO` still works), backed by a scan service that reuses IntelliJ's native PSI TODO index instead of re-scanning.
- Enhanced tool window: a sortable, filterable table (type, priority, assignee, tag, free-text, "Only mine") with double-click jump-to-code and debounced auto-refresh on save.
- Iterated the UI from a table into a modern widget — rounded card toolbar, theme-aware priority pill badges, and a cyclable "stack of cards" (prev/next via buttons, arrow keys, or mouse-wheel), with an option to float it as a sticky-note window.
- Automated release pipeline: Gradle plugin signing plus a GitHub Actions workflow that builds and packages a signed artifact on each release.

### 🧰 [Asad's Toolbox](https://github.com/asadsq/intellij-plugin) — IntelliJ IDEA productivity plugin
`Kotlin` · `IntelliJ Platform Gradle Plugin 2.x` · `IDEA 2025.2` · `GitHub Actions`

A grab-bag of quality-of-life additions for the IDE, built on the JetBrains Platform template with CI and Plugin Verifier passing across four IDE builds.

🎤 *My first attempt at building something for the JetBrains conference — a collection of ideas and experiments that eventually pointed the way to jb-todo-enhancer.*

- **Folder Highlighter** — tints every file and subfolder inside the selected Project-view folder so its contents are visually unambiguous despite deep indentation (a `ProjectViewNodeDecorator` with `VfsUtilCore` ancestor checks and live re-render on tree selection).
- **DocuSign-style "Jump to Next Diff" pill** for the diff/commit view — ▲/▼ navigation, a live change count, and first/last auto-disable, delegating to the platform's native diff navigation so it stays in sync with F7 and the gutter markers.
- Cleared the Plugin Verifier gate in part by replacing a non-public navigation call with the platform's registered `NextDiff`/`PreviousDiff` actions.

### ⭐ [reward-jar](https://github.com/asadsq/reward-jar) — SwiftUI iOS app
`Swift` · `SwiftUI`

A SwiftUI app for toddlers that encourages reward-based parenting — collect stars and gems, fill the jar, earn a reward.

- Animated "reward jar" with live counters and celebration animations, built entirely from custom cartoon shapes, a central color palette, code-drawn backgrounds, and in-code synthesized sound (no audio assets).
- Structured into focused SwiftUI components (Jar, JarItem, Counters, Celebration, CartoonShapes, SoundManager, …), developed with a disciplined Git workflow: develop-based feature branches in isolated worktrees, pull requests, and post-merge branch cleanup.

---

## Also on my profile

Beyond the projects above, my profile holds **28 repositories** in total — a trail of learning projects and experiments picked up over the years. Relics from the pre-agent era. A few worth a look, grouped by theme:

**iOS / Swift** — apps and Xcode experiments

- **[ios-clima](https://github.com/asadsq/ios-clima)** — a weather app that pulls live conditions for a city or your current location.
- **[ios-quizzler](https://github.com/asadsq/ios-quizzler)** — a quiz game exploring Swift structs, optionals, and view state.
- **[ios-flash-chat](https://github.com/asadsq/ios-flash-chat)** — a chat app with user login and a live message feed.
- **[ios-Todoey](https://github.com/asadsq/ios-Todoey)** — a to-do app for tracking items, inspired by the Clear app.
- **[ios-xylophone](https://github.com/asadsq/ios-xylophone)** — a tap-to-play xylophone exploring audio playback.
- **[ios-bitcoin-tick](https://github.com/asadsq/ios-bitcoin-tick)** — a Bitcoin price ticker fetching live rates across currencies (CocoaPods, networking, JSON).
- **[hello-ios-app](https://github.com/asadsq/hello-ios-app)** — a "hello world" first Xcode app, knocking the rust off after years away.

**Front-end web** — HTML/CSS/JS and Node mini-projects

- **[web-drumkit](https://github.com/asadsq/web-drumkit)** — a browser drum kit that triggers sounds on key press and click.
- **[web-Dicee](https://github.com/asadsq/web-Dicee)** — a two-player dice-roll game in vanilla JavaScript.
- **[web-calculator](https://github.com/asadsq/web-calculator)** — a small HTML/CSS/JS calculator.
- **[web-newsletter](https://github.com/asadsq/web-newsletter)** — a newsletter signup form backed by a Node.js server.
- **[web-ejs-challenge](https://github.com/asadsq/web-ejs-challenge)** — an Express + EJS server-side templating exercise.
- **[web-todo-list-v1](https://github.com/asadsq/web-todo-list-v1)** / **[web-to-do-list-v2](https://github.com/asadsq/web-to-do-list-v2)** — two iterations of a to-do web app, from a static first pass to a dynamic version.
- **[web-fruits](https://github.com/asadsq/web-fruits)** — a Node.js exercise in data modeling and persistence.

**DevOps / Docker** — containerization and CI experiments

- **[devops-complex](https://github.com/asadsq/devops-complex)** — a multi-container app (client / server / worker / nginx) wired for Docker Compose, Travis CI, and AWS Elastic Beanstalk.
- **[devops-frontend](https://github.com/asadsq/devops-frontend)** — a Create React App front-end containerized with dev/prod Dockerfiles and a Travis CI pipeline.
- **[devops-visits](https://github.com/asadsq/devops-visits)** — a small Node service used as the app tier in a Dockerized visit-counter demo.
- **[devops-simpleweb](https://github.com/asadsq/devops-simpleweb)** — a minimal web service focused on writing a first Dockerfile and image build.

**Coursework & misc**

- **[misc-umich-481](https://github.com/asadsq/misc-umich-481)** — coursework from EECS 481 (Software Engineering) at the University of Michigan.
- **[misc-mean-course](https://github.com/asadsq/misc-mean-course)** — a MEAN-stack (MongoDB / Express / Angular / Node) project in TypeScript.
- **[misc-chrome-extension](https://github.com/asadsq/misc-chrome-extension)** — a Chrome browser extension with a popup UI (manifest, HTML/CSS/JS).

---

<sub>📍 Dallas–Fort Worth, TX · Let's connect → asadsq@umich.edu</sub>
