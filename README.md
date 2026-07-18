# Hi, I'm Asad 👋

Tech lead with **12+ years** building enterprise software that runs on the cloud. Most of my day job is deep in Java, AWS, and distributed systems — lately with a focus on **LLM integration** into production pipelines. Off the clock, I build developer tools and small apps, usually pairing spec-driven, agent-augmented workflows with real engineering rigor: tests, code review, CI, and verification gates.

- 🔭 Currently: Tech Lead at CorroHealth, working on LLM-driven medical-coding accuracy and real-time anomaly detection at fleet scale (1,500+ nodes).
- 🧰 For fun: MCP servers, IntelliJ plugins, and SwiftUI apps — the pinned repos below.
- 🎓 B.S. Computer Science, University of Michigan, Ann Arbor.
- 📫 Reach me: asadsq@umich.edu

### Tech I work with

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

`Java` · `AWS (SDK, EC2, S3, SQS, Lambda)` · `REST APIs` · `Spring Boot` · `LLM integration` · `Gradle / Maven` · `Rundeck · Jenkins` · `Dynatrace · Loggly · PagerDuty`

---

## Featured projects

### 🗺️ [Cartograph](https://github.com/asadsq/cartograph-mcp-server) — MCP server for AI-agent codebase review
`Java 21` · `Maven` · `Model Context Protocol SDK 2.0` · `JUnit 5` · `GitHub Actions`

A Model Context Protocol server that gives AI coding agents a complete, queryable map of a codebase's dependency and call graph — exhaustive, deterministic answers to whole-graph questions that agents can't reliably reconstruct by grep-and-read alone.

- Complete **blast-radius** analysis (full transitive closure of dependents, grouped by distance), circular-dependency detection, in-degree "hotspot" ranking, and shortest dependency path between modules.
- Every tool explains what it did in plain English, with honest resolved-vs-unresolved coverage reporting — trust over false precision.
- **Privacy-first, local-only** deployment: runs entirely on your machine, so proprietary source never leaves it.
- Ships as a shaded, runnable JAR with JUnit 5 tests, MCP Inspector verification, and GitHub Actions CI.

### ✅ [jb-todo-enhancer](https://github.com/asadsq/jb-todo-enhancer) — IntelliJ IDEA plugin
`Kotlin` · `IntelliJ Platform Gradle Plugin 2.x` · `IDEA 2025.2` · `JUnit 5` · `GitHub Actions`

Upgrades IntelliJ's built-in TODO handling. Scoped in plan mode as a weekly MVP, with 13 unit tests, CI, and Plugin Verifier compatibility across four IDE builds (2025.2–2026.2).

- Structured TODO syntax — `// TODO(@asad) !p1 #backend due:2026-07-10` — parsing assignee, priority, tags, and due date (plain `// TODO` still works), backed by a scan service that reuses IntelliJ's native PSI TODO index instead of re-scanning.
- Enhanced tool window: a sortable, filterable table (type, priority, assignee, tag, free-text, "Only mine") with double-click jump-to-code and debounced auto-refresh on save.
- Iterated the UI from a table into a modern widget — rounded card toolbar, theme-aware priority pill badges, and a cyclable "stack of cards" (prev/next via buttons, arrow keys, or mouse-wheel), with an option to float it as a sticky-note window.
- Automated release pipeline: Gradle plugin signing plus a GitHub Actions workflow that builds and packages a signed artifact on each release.

### 🧰 [Asad's Toolbox](https://github.com/asadsq/intellij-plugin) — IntelliJ IDEA productivity plugin
`Kotlin` · `IntelliJ Platform Gradle Plugin 2.x` · `IDEA 2025.2` · `GitHub Actions`

A grab-bag of quality-of-life additions for the IDE, built on the JetBrains Platform template with CI and Plugin Verifier passing across four IDE builds.

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

A few older learning and portfolio repos worth a look:

- **[ios-bitcoin-tick](https://github.com/asadsq/ios-bitcoin-tick)** — a Swift Bitcoin price ticker fetching live rates across currencies; CocoaPods, networking, and JSON parsing.
- **[devops-complex](https://github.com/asadsq/devops-complex)** — a multi-container web app (client / server / worker / nginx) wired for Docker Compose, Travis CI, and AWS Elastic Beanstalk deployment.

---

<sub>📍 Dallas–Fort Worth, TX · Let's connect → asadsq@umich.edu</sub>
