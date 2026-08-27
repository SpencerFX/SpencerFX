# Spencer P

Senior KDB+ Developer and Data Scientist with 8+ years of experience building
high-performance kdb+/q tick-database and market-data infrastructure —
tickerplant/RDB/HDB architectures, real-time and historical data pipelines,
feed handlers, and the testing/tooling that keeps them reliable. Also works
in Python and C/C++ for data pipelines and native q extensions.

Active open-source contributor and tooling author.

## Open Source Projects

### Platform

- [openQ](https://github.com/SpencerFX/openQ) [Public] A lightweight, domain-generic kdb+ tick-database core 
- [fxDB](https://github.com/SpencerFX/fxDB) [Private] A complete kdb+/q FX tick-database

### Ingestion

- [ampsQ](https://github.com/SpencerFX/ampsQ) [Public] Extension embedding the 60East AMPS C++ client behind a C API
- [edinetToKdb](https://github.com/SpencerFX/edinetToKdb) [Public] EDINET (Japan financial disclosure) data into kdb+

### Integration

- [lean-kdb](https://github.com/SpencerFX/lean-kdb) [Public] Integration layer for the open-source QuantConnect LEAN engine

### Community

- [q-link](https://github.com/SpencerFX/q-link) [Public] code companion repo for LinkedIn articles on kdb+/q
- [q-Quiz](https://github.com/SpencerFX/q-Quiz) [Public] coding practice and interview prep, mostly in q

### Trading Strategy

- [Algorithmic-Trading-Strategies](https://github.com/SpencerFX/Algorithmic-Trading-Strategies) [Public] Momentum-based trading strategy coded in Lua

### Library

- [q-test](https://github.com/SpencerFX/q-test) [Public] a kdb+/q testing framework built by studying four existing ones (qunit, q-unit, qspec, resq) plus q-desc's fuzz-test generator
- [qlearing](https://github.com/SpencerFX/qlearing) [Public] a kdb+/q library for clearing-related processing
- [q-gis](https://github.com/SpencerFX/q-gis) [Public] kdb+/q geospatial tooling

## Interview Prep

- [HackerRankQ](https://github.com/SpencerFX/HackerRankQ) [Public] - Solutions in Q
- [leetcodeQ](https://github.com/SpencerFX/leetcodeQ) [Public] - Solutions in Q
- [interviewQ](https://github.com/SpencerFX/interviewQ) [Public] - General Interview questions

## Math Studies

- [eulerQ](https://github.com/SpencerFX/eulerQ) [Public] - Solutions in Q
- [matrixAlgebraForEngineersQ](https://github.com/SpencerFX/matrixAlgebraForEngineersQ) [Public] - HKUST course in q
- [q-math-calculus](https://github.com/SpencerFX/q-math-calculus) [Public] self-study notes and exercises in kdb+/q
- [Itarle-Challenge](https://github.com/SpencerFX/Itarle-Challenge) [Public] a quant recruitment take-home exercise

## Roadmap

| Repo | Progress | Roadmap |
| ---- | -------- | ------- |
| [openQ](https://github.com/SpencerFX/openQ) | Working tick pipeline (TP/RDB/HDB/gateway/CEP/tmphdb); 20 integration checks passing; can front an existing on-disk HDB read-only | Shared `.oq.sub.*` subscribe helper to dedup RDB/CEP/tmphdb; live WebSocket feed handler (blocked on local kdb+ build); wire up openDash |
| [fxDB](https://github.com/SpencerFX/fxDB) | Complete private FX tick-database; the production reference openQ is distilled from | Maintenance only; fold hardened features back into openQ |
| [ampsQ](https://github.com/SpencerFX/ampsQ) | C ABI + q API implemented; off-thread `eventfd` → `sd1()` delivery; publish/subscribe example scripts | CI build against the AMPS SDK; reconnect/failover; bookmark (replay) subscriptions; broaden past Linux x86-64 |
| [edinetToKdb](https://github.com/SpencerFX/edinetToKdb) | Python download + parse pipeline loading EDINET disclosures into kdb+ | Add README/usage docs; incremental sync; cover more disclosure form types |
| [lean-kdb](https://github.com/SpencerFX/lean-kdb) | Phase 1: C# `KdbPlus` history provider + q gateway; `dotnet test` 2/2, q side verified locally | End-to-end run via Docker/WSL2; real-time data feed; brokerage/order routing |
| [q-link](https://github.com/SpencerFX/q-link) | 3 published articles with runnable code and hard-assert test runners (markout/impact, spread decomposition, table logging) | More articles; shared synthetic-data harness across pieces |
| [q-Quiz](https://github.com/SpencerFX/q-Quiz) | Flask + q judge across 8 coding sections, quizzes and timed assessments; supervisor with auto-restart + autosave; pytest suite | Multi-user auth; containerized multi-service (q-core / judge-worker / web) K8s deploy; more problem sets |
| [Algorithmic-Trading-Strategies](https://github.com/SpencerFX/Algorithmic-Trading-Strategies) | Momentum strategy implemented in Lua | Backtest through lean-kdb; add q-side analytics |
| [q-test](https://github.com/SpencerFX/q-test) | ~700-line pure-q engine; xUnit + BDD DSLs on one core, auto-restoring mocks, property tests with shrinking, test scaffolding and schema-aware data generation; self-tested 13/13 | Richer type-driven generators; coverage reporting; parallel / sharded runs |
| [qlearing](https://github.com/SpencerFX/qlearing) | Early — clearing-processing library skeleton | Core netting / settlement / margin calcs; worked examples and tests |
| [q-gis](https://github.com/SpencerFX/q-gis) | Early — geospatial tooling, pre-README | Document the API; spatial joins / indexing; sample datasets |
| [HackerRankQ](https://github.com/SpencerFX/HackerRankQ) | 23 easy problems solved, ~50+ tracked | Finish the easy tier, then medium/hard; data-structures and FP sections |
| [leetcodeQ](https://github.com/SpencerFX/leetcodeQ) | Problems 1–5 solved, tracker out to 58+ | Work the top-150; group solutions by pattern |
| [interviewQ](https://github.com/SpencerFX/interviewQ) | Question collection, pre-README | Organize by topic; add model answers in q |
| [eulerQ](https://github.com/SpencerFX/eulerQ) | Project Euler solutions in q | Continue; capture reusable idioms in the phrasebook |
| [matrixAlgebraForEngineersQ](https://github.com/SpencerFX/matrixAlgebraForEngineersQ) | Weeks 1–3 complete, Week 4 in progress | Finish remaining course weeks; eigenvalues / PCA |
| [q-math-calculus](https://github.com/SpencerFX/q-math-calculus) | Self-study notes and exercises | Numerical differentiation / integration; ODE examples |
| [Itarle-Challenge](https://github.com/SpencerFX/Itarle-Challenge) | Quant take-home: per-stock tick statistics (spreads, inter-trade/tick times, round-number effect) in Python | q port; tighten auction-exclusion edge cases |

## Programming Languages

| Language | Level  |
| -------- | ------ |
| q        | Expert |
| kdb+     | Expert |
| Python   | Expert |
| C/C++    | Interm |
| Shell    | Expert |
