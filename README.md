<div align="center">

**Software Engineer · Go Open-Sourcer · GenAI Community Leader · Hackathon Organizer**

📍 Nantes, France &nbsp;&nbsp;|&nbsp;&nbsp; 🌐 [samuel-berthe.fr](http://samuel-berthe.fr/) &nbsp;&nbsp;|&nbsp;&nbsp; 📝 [Substack](https://samuelberthe.substack.com/) &nbsp;&nbsp;|&nbsp;&nbsp; 🐦 [@samuelberthe](https://twitter.com/samuelberthe) &nbsp;&nbsp;|&nbsp;&nbsp; 🦋 [@samber.bsky.social](https://bsky.app/profile/samber.bsky.social) &nbsp;&nbsp;|&nbsp;&nbsp; 💼 [LinkedIn](https://www.linkedin.com/in/samuelberthe/)

<img alt="image" src="https://github.com/user-attachments/assets/37a4f806-1361-47b6-b7a7-92c544f56b3a" />

</div>

<br>

Hi. I'm Samuel. I write Go libraries. It started as a hobby, turned into a side project, and is now my attempt at making open source a full-time job. The jury is still out. The coffee budget is not.

It began the usual way: I needed something at work that didn't exist, built it, and thought "someone else probably needs this too." That pattern never stopped. The most well-known result is **[lo](https://github.com/samber/lo)**, a utility library built on Go generics. It's now used in production at companies of all sizes, such as RedHat, VMware, Tencent, Bytedance, Grafana, and many others.

Adoption comes with perks: AI-slop PRs, and the rare keyboard warrior ready to die on a typo 🙃. But honestly? The community around these projects is overwhelmingly kind, sharp, and generous. And I'm grateful for every single one of you. 💖

The ecosystem kept growing from there: monads, dependency injection, caching, structured errors, and **35+ `log/slog` handlers**. If your stack uses Terraform, Kubernetes, the Grafana stack, apps you've definitely opened today (if you're Chinese), or a few places you'd rather not think about 😅 #pr0n — there's a fair chance my code is already quietly running somewhere.

On the community side: I started the [Generative AI meetup in Nantes (Fr)](https://www.meetup.com/generative-ai-nantes) from scratch: no audience, no budget, no certainty anyone would show up. It became the largest GenAI meetup in France 🇫🇷. I also run [hackathons](https://shift-hackathon.com/), [speak at conferences](https://github.com/samber/talks), and write on [Substack](https://samuelberthe.substack.com/).

If your team ships with any of my libraries and you want to help me keep doing this, [sponsoring on GitHub](https://github.com/sponsors/samber) goes a long way. No SLA included, but bugs get fixed with genuine enthusiasm.

My lifetime goal? `git push --force` into a satellite. Just kidding. Well... maybe not entirely.

---

## The Go Toolkit

Turns out Go generics unlock a lot. I'm still finding out how much.

| Library                                  | What it does                                                   |
| ---------------------------------------- | -------------------------------------------------------------- |
| 🔧 **[lo](https://github.com/samber/lo)** | Lodash-style helpers for Go: Map, Filter, Reduce, and 90+ more |
| 🌀 **[mo](https://github.com/samber/mo)** | Monads for Go: Option, Result, Either, Future                  |
| ⚙️ **[do](https://github.com/samber/do)** | Dependency injection with generics for Go                      |
| 🌊 **[ro](https://github.com/samber/ro)** | Reactive streams & event-driven programming for Go             |

Be aware, 22 letters left for my next Go projects. Plenty of runway. 😂😂😂

At this pace I'll own the entire alphabet before Go drops `GOPATH` from the docs.

---

## The Go slog Ecosystem

Go 1.21 introduced `log/slog` as the standard structured logger. I built **35+ handlers** so you only configure slog once and route logs anywhere:

At some point "just one more handler" stopped being a joke. When you have 1, the next 42 come effortlessly.

**Core**

| Project                                                          | Description                                                       |
| ---------------------------------------------------------------- | ----------------------------------------------------------------- |
| 🔀 **[slog-multi](https://github.com/samber/slog-multi)**         | Fanout, pipeline, routing, and failover between multiple handlers |
| 🎨 **[slog-formatter](https://github.com/samber/slog-formatter)** | Attribute formatting and transformation                           |
| 🎲 **[slog-sampling](https://github.com/samber/slog-sampling)**   | Log sampling policies to reduce high-volume noise                 |
| 🃏 **[slog-mock](https://github.com/samber/slog-mock)**           | Mock handler for unit testing                                     |

**HTTP middleware** — [slog-gin](https://github.com/samber/slog-gin) · [slog-echo](https://github.com/samber/slog-echo) · [slog-fiber](https://github.com/samber/slog-fiber) · [slog-chi](https://github.com/samber/slog-chi) · [slog-http](https://github.com/samber/slog-http)

**Monitoring & observability** — [slog-logstash](https://github.com/samber/slog-logstash) · [slog-syslog](https://github.com/samber/slog-syslog) · [slog-fluentd](https://github.com/samber/slog-fluentd) · [slog-loki](https://github.com/samber/slog-loki) · [slog-datadog](https://github.com/samber/slog-datadog) · [slog-sentry](https://github.com/samber/slog-sentry) · [slog-otel](https://github.com/samber/slog-otel) · [slog-graylog](https://github.com/samber/slog-graylog) · [slog-quickwit](https://github.com/samber/slog-quickwit) · [slog-rollbar](https://github.com/samber/slog-rollbar) · [slog-betterstack](https://github.com/samber/slog-betterstack)

**Notifications** — [slog-slack](https://github.com/samber/slog-slack) · [slog-telegram](https://github.com/samber/slog-telegram) · [slog-webhook](https://github.com/samber/slog-webhook) · [slog-mattermost](https://github.com/samber/slog-mattermost) · [slog-microsoft-teams](https://github.com/samber/slog-microsoft-teams)

**Messaging & streaming** — [slog-kafka](https://github.com/samber/slog-kafka) · [slog-nats](https://github.com/samber/slog-nats) · [slog-channel](https://github.com/samber/slog-channel) · [slog-parquet](https://github.com/samber/slog-parquet)

**Adapters** — [slog-zap](https://github.com/samber/slog-zap) · [slog-zerolog](https://github.com/samber/slog-zerolog) · [slog-logrus](https://github.com/samber/slog-logrus)

---

## Go Utilities

The stuff that didn't fit anywhere else but was too useful to delete.

| Project                                                                  | Description                                                                                          |
| ------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------- |
| 💥 **[oops](https://github.com/samber/oops)**                             | Errors with context, stack traces, and structured metadata                                           |
| 🔥 **[hot](https://github.com/samber/hot)**                               | In-memory cache: LRU, LFU, TinyLFU, W-TinyLFU, ARC, 2Q, S3FIFO, SIEVE, FIFO, N-random; TTL, sharding |
| 🕸️ **[go-mod-graph](https://github.com/samber/go-mod-graph)**             | Web-based Go module dependency graph visualizer                                                      |
| 🐰 **[go-amqp-pubsub](https://github.com/samber/go-amqp-pubsub)**         | Resilient pub/sub framework for RabbitMQ, auto-reconnects and binds on network failure               |
| 🔁 **[go-singleflightx](https://github.com/samber/go-singleflightx)**     | `x/sync/singleflight` with generics and an extended API                                              |
| 📦 **[go-batchify](https://github.com/samber/go-batchify)**               | Group and deduplicate concurrent tasks to reduce downstream load                                     |
| 🔤 **[go-type-to-string](https://github.com/samber/go-type-to-string)**   | Extract a string representation of any Go type                                                       |
| 📏 **[go-metered-stream](https://github.com/samber/go-metered-stream)**   | Drop-in `io.Reader`/`io.Writer` that tracks total bytes transferred                                  |
| 🔌 **[go-tcp-pool](https://github.com/samber/go-tcp-pool)**               | TCP connection pool with auto-reconnect as a `net.Conn` drop-in                                      |
| 📊 **[go-psi](https://github.com/samber/go-psi)**                         | Linux Pressure Stall Information (PSI) reader and starvation notifier                                |
| 🔍 **[go-quickwit](https://github.com/samber/go-quickwit)**               | Go ingestion client for Quickwit search engine                                                       |
| 🛡️ **[go-safe-csv-writer](https://github.com/samber/go-safe-csv-writer)** | `encoding/csv` fork that prevents CSV injection and data exfiltration                                |

---

## Claude Code / AI Tooling

AI-native tooling built by someone who spends way too much time inside the tool. You know... dopamine...

| Project                                                                          | Description                                                                |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| 🛠️ **[cc](https://github.com/samber/cc)**                                         | Claude Code toolchain and marketplace                                      |
| ☕ **[cc-caffeine](https://github.com/samber/cc-caffeine)**                       | Keep Claude Code alive while commuting, prevents laptop sleep              |
| 🧠 **[cc-skills](https://github.com/samber/cc-skills)**                           | Reusable AI agent skills for marketing and engineering                     |
| 🐹 **[cc-skills-golang](https://github.com/samber/cc-skills-golang)**             | AI agent skills purpose-built for production Go projects                   |
| 🤖 **[go-playground-mcp](https://github.com/samber/go-playground-mcp)**           | MCP server for Go Playground, run and share Go code from your AI assistant |
| 🛡️ **[the-great-gpt-firewall](https://github.com/samber/the-great-gpt-firewall)** | Curated list of sites blocking AI crawlers via `robots.txt`                |
| 🔢 **[tiktoken-cli](https://github.com/samber/tiktoken-cli)**                     | Count LLM tokens in files and directories from the terminal                |
| 📊 **[vscode-token-counter](https://github.com/samber/vscode-token-counter)**     | VS Code extension showing live token counts in the status bar              |

---

## Awesome Collections

Lists of things so you don't have to ChatGPT them at 2am.

| Project                                                                                | Description                                                       |
| -------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| ⚡ **[awesome-prometheus-alerts](https://github.com/samber/awesome-prometheus-alerts)** | 1.000 production-ready Prometheus alerting rules for 100 services |
| 📊 **[awesome-olap](https://github.com/samber/awesome-olap)**                          | Curated list of OLAP databases and analytical query engines       |
| 🫟 **[awesome-user-research](https://github.com/samber/awesome-user-research)**        | Curated list of tools for Product Managers and UX Researchers     |

---

## Prometheus & Observability

If you can't measure it, you can't get paged on it at 3am.

Alert on everything. Sleep on nothing.

| Project                                                                                                      | Description                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| ⚡ **[awesome-prometheus-alerts](https://github.com/samber/awesome-prometheus-alerts)**                       | 1.000 production-ready Prometheus alerting rules for 100 services                                                               |
| 📊 **[prometheus-query-js](https://github.com/samber/prometheus-query-js)**                                   | JavaScript client for the Prometheus HTTP query API                                                                             |
| 📈 **[chartjs-plugin-datasource-prometheus](https://github.com/samber/chartjs-plugin-datasource-prometheus)** | Prometheus datasource plugin for Chart.js                                                                                       |
| 📤 **[promql-exporter](https://github.com/samber/promql_exporter)**                                           | Prometheus exporter that re-exposes PromQL query results as metrics (replacing federation and remote-write for niche use-cases) |
| 🏓 **[hyperping-exporter](https://github.com/samber/hyperping-exporter)**                                     | Prometheus exporter for Hyperping uptime monitoring                                                                             |
| ☁️ **[clevercloud-exporter](https://github.com/samber/clevercloud-exporter)**                                 | Prometheus exporter for Clever Cloud infrastructure metrics                                                                     |

---

## Tools & Utilities

Random things? Maybe. Useless? Never.

| Project                                                                      | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| 🧾 **[invoice-as-a-service](https://github.com/samber/invoice-as-a-service)** | Generate professional PDF invoices from a single HTTP POST, with S3 upload   |
| 📝 **[headercheck](https://github.com/samber/headercheck)**                   | Linter that checks and fixes required file headers, golangci-lint compatible |
| 🔑 **[sync-ssh-keys](https://github.com/samber/sync-ssh-keys)**               | Sync server `~/.ssh/authorized_keys` from GitHub/GitLab org membership       |
| 🔀 **[git-contrib-graph](https://github.com/samber/git-contrib-graph)**       | Git contribution graph rendered in the terminal                              |

---

## Writing & Talks

Occasionally I stop writing code long enough to write words about code, with live demo that goes exactly as planned.

**[Substack](https://samuelberthe.substack.com/)** - I write about Go, open-source, and software engineering on Substack. Deep dives into performance engineering, library design, and lessons learned from maintaining high-traffic OSS projects.

**[Talks](https://github.com/samber/talks)** - Slides and resources from my conference talks and meetup presentations. Topics include generative AI, performance engineering, observability, Golang, and building open-source communities.

**[Generative AI meetup replays 🇫🇷](https://www.youtube.com/watch?v=8UWCLts47Ms&list=PL6lvFX2OvdHupZLKOPIzy-ZCdA6AnlFYb)** - When my camera does not crash in the middle of the talk.

---

## 🚀 Fuel My Work

All those green squares, and yet rent is still due every month.

> My open-source libraries ship in production at companies of all sizes, maybe yours too.
> Sponsorship keeps the libraries maintained, documented, and evolving.

<div align="center">

| What your sponsorship funds    |                                                            |
| ------------------------------ | ---------------------------------------------------------- |
| 🐛 Bug fixes & security patches | Rapid response to issues affecting production systems      |
| 📖 Documentation & examples     | Real-world patterns, migration guides, and tutorials       |
| 🔬 New features & research      | Exploring what Go can do next                              |
| 🌍 Community support            | Answering questions, reviewing PRs, mentoring contributors |

[![Become a sponsor](https://img.shields.io/badge/Become_a_Sponsor-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/samber)

### 💎 Corporate Sponsorship Tiers

Ideal for teams that depend on `lo`, `mo`, `do`, `oops`, or `awesome-prometheus-alerts` in production.

| Tier                     | Benefit                                                  |
| ------------------------ | -------------------------------------------------------- |
| ☕️ **Individual backers** | Fuel the coffee machine                                  |
| 🥉 **Insider**            | Private channel + early access + roadmap vote            |
| 🥈 **Supporter**          | Logo in sponsored repos (READMEs and websites)           |
| 🥇 **Partner**            | Logo everywhere + priority issue response + co-marketing |

[![Contact for partnership](https://img.shields.io/badge/Contact_for_Partnership-0077B5?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hey@samuel-berthe.fr)

</div>

### 🙏 Thank You, Sponsors

<div align="center">

**[DBOS](https://www.dbos.dev/?utm_campaign=gh-smbr)** · **[Better Stack](https://betterstack.com/)** · **[Dash0](https://www.dash0.com/?utm_campaign=148395251-samber%20github%20sponsorship&utm_source=github&utm_medium=sponsorship&utm_content=samber)** · **[CAST AI](https://cast.ai/samuel)**

</div>

<div align="center">

<img width="1" src="https://visitor-badge.laobi.icu/badge?page_id=samber.samber&style=flat-square">
<!-- ![Visitor Count](https://visitor-badge.laobi.icu/badge?page_id=samber.samber&style=flat-square) -->

</div>
