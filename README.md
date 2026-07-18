<!-- ============================================================
     Roshan Raj — GitHub profile README (roshworldwide/roshworldwide)
     Liquid-Glass banners are rendered PNGs (see /assets + *.html sources).
     Everything else is GitHub-native Markdown so links stay live.
     ============================================================ -->

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)"  srcset="assets/header-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/header-light.svg">
    <img alt="Roshan Raj — First-Principles Systems Engineer & AI-Infrastructure Architect. Ships production systems most teams only prototype. 330K writes/second · 142M+ states formally verified · 99.9% uptime for 5,000+ users · 7 patents pending." src="assets/header-dark.svg" width="100%">
  </picture>
</div>

<p align="center">
  <a href="https://roshworldwide.com"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-roshworldwide.com-0A84FF?style=flat-square&logo=safari&logoColor=white"></a>
  <a href="mailto:roshan@roshworldwide.com"><img alt="Email" src="https://img.shields.io/badge/Email-roshan@roshworldwide.com-5E5CE6?style=flat-square&logo=maildotru&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/roshworldwide"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-in%2Froshworldwide-0A66C2?style=flat-square&logo=linkedin&logoColor=white"></a>
  <img alt="Location" src="https://img.shields.io/badge/Bengaluru-India-8A8A94?style=flat-square&logo=googlemaps&logoColor=white">
  <img alt="Open to senior / infra roles" src="https://img.shields.io/badge/Open_to-Senior%20%2F%20Infra%20roles-30D158?style=flat-square">
</p>

## ⚙️ Flagship work

Systems built from first principles — storage engines, inference runtimes, and formally-verified infrastructure, written mostly in Rust and benchmarked against real baselines.

**[Engram](https://github.com/roshworldwide/engram)** &nbsp;·&nbsp; AI-Agent Memory Storage Engine
Four native memory types, bitemporal time-travel, and a causal-provenance DAG on a custom copy-on-write B-tree + WAL (MVCC).
`330K durable writes/s` `165× faster time-travel vs Postgres` `93% coverage` `4 fuzz targets × 10M runs`
<sub>**Rust** · COW B-tree · WAL/MVCC · PyO3 SDK · VLDB-style paper draft</sub>

**[Crucible](https://github.com/roshworldwide/crucible)** &nbsp;·&nbsp; Air-Gapped Multi-Tenant LLM Inference Runtime
A hand-written transformer stack across 13 crates — attention, paged KV cache, continuous batching, speculative decoding. Zero PyTorch / BLAS / Python (CI-enforced).
`13 crates` `NEON GEMM ~3× scalar` `Metal kernels` `AES-256 per-tenant isolation`
<sub>**Rust** · NEON SIMD · Metal · paged KV cache · property-tested non-interference</sub>

**[Axiom](https://github.com/roshworldwide/axiom)** &nbsp;·&nbsp; Formally-Verified CRDT Runtime
TLA+ specs for four CRDTs model-checked across 142M+ states, plus two machine-checked TLAPS proofs. Rust bound to specs via refinement mappings & trace replay.
`142M+ states checked` `2 TLAPS proofs` `4 CRDTs` `anti-replay freshness proven`
<sub>**TLA+ / TLAPS** · Rust · refinement mappings · trace replay</sub>

**[Holdout](https://github.com/roshworldwide/holdout)** &nbsp;·&nbsp; LLM Evaluation Framework &nbsp;`open source`
A CI regression gate with statistical rigor: BCa bootstrap CIs, McNemar / permutation tests, Benjamini–Hochberg correction, power / MDE, and leakage detection.
`4 backends` `fully offline` `1,000+ cases/run` `~6 µs overhead`
<sub>**Python** · pytest plugin · GitHub Action · OpenAI · Anthropic · Ollama · Apple MLX</sub>

**On-Premise SRE Engine** &nbsp;·&nbsp; Autonomous air-gapped incident response
Runs a 14B-parameter 4-bit LLM fully air-gapped — 0 bytes outbound. A digital-twin sandbox detects microservice anomalies and auto-generates Kubernetes / Bash remediations in under 800 ms, while a 120 fps GPU frontend tracks $10K+/min outage burn.
`14B params · 4-bit` `0 bytes outbound` `<800 ms remediation` `120 fps GPU frontend`
<sub>Air-gapped LLM · digital-twin sandbox · Kubernetes · GPU rendering</sub>

## ⚡ Live demos

Two shipped products, both running live on GitHub Pages:

- **Sahayak** — an offline, vernacular AI fraud-shield for Bharat. → **[Try it live ↗](https://roshworldwide.github.io/optum-v2/)**
- **Pramaan** — verifiable carbon MRV; watch a tampered reading get rejected. → **[Try it live ↗](https://roshworldwide.github.io/optum-v3/)**

## 📜 7 patents pending

Novel systems spanning authentication, collaboration, privacy, and human–computer interaction.

`01` Acoustic Proximity Authentication &nbsp;·&nbsp; `02` Negative-Latency Collaborative Editing &nbsp;·&nbsp; `03` Semantic Clipboard &nbsp;·&nbsp; `04` Privacy-Preserving Crash Reproduction &nbsp;·&nbsp; `05` On-Device Pre-Update Regression Certification &nbsp;·&nbsp; `06` Unified Fidelity-Budget Scheduler &nbsp;·&nbsp; `07` Dynamically Morphing Ergonomic Keyboard

## 🧭 Experience

**Co-Founder & Lead Engineer** &nbsp;·&nbsp; Bastian Build &nbsp;·&nbsp; <sub>Jan – Apr 2026</sub>
Invented **Acoustic AMS**, a campus-wide attendance system on an acoustic-handshake protocol that defeats GPS / Bluetooth relay & spoofing — sub-50 ms verify, 99.9% uptime for 5,000+ students, scaling B2B to 4–5 campuses. Ran a zero-downtime migration of 31 Postgres tables to a serverless Supabase / Vercel stack.

**Data Analyst Intern** &nbsp;·&nbsp; Convin.ai &nbsp;·&nbsp; <sub>2026</sub>
Built the live analytics platform quantifying **₹5.5 Cr+/day** recovered in a client bank's collections; rebuilt the audit workflow as a dedicated app (~10× faster, 4,000–6,000 audits/month). Both adopted company-wide.

**Software Engineering Intern · AI FinTech** &nbsp;·&nbsp; Lenn Chartered &nbsp;·&nbsp; <sub>Mar – May 2026</sub>
Fine-tuned a domain FinTech LLM into a production advisor (query-resolution **−90%** with regulatory accuracy); built a low-latency synthetic paper-trading engine for 5,000+ concurrent users.

**Full-Stack Developer** &nbsp;·&nbsp; OxyHarvest &nbsp;·&nbsp; <sub>Dec 2025 – Feb 2026</sub>
Shipped the live impact platform streaming real-time CO₂ telemetry from 90+ deployed purifiers via Xano APIs, plus the field apps used by 30 technicians.

## 🧠 Toolbox

**Languages** &nbsp;
![Rust](https://img.shields.io/badge/Rust-0A84FF?style=flat-square&logo=rust&logoColor=white) ![Python](https://img.shields.io/badge/Python-0A84FF?style=flat-square&logo=python&logoColor=white) ![Swift](https://img.shields.io/badge/Swift-0A84FF?style=flat-square&logo=swift&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-0A84FF?style=flat-square&logo=typescript&logoColor=white) ![C/C++](https://img.shields.io/badge/C%20%2F%20C%2B%2B-0A84FF?style=flat-square&logo=cplusplus&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-0A84FF?style=flat-square&logo=postgresql&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-0A84FF?style=flat-square&logo=gnubash&logoColor=white) ![TLA+](https://img.shields.io/badge/TLA%2B-0A84FF?style=flat-square)

**ML & LLMs** &nbsp;
![PyTorch](https://img.shields.io/badge/PyTorch-9127C4?style=flat-square&logo=pytorch&logoColor=white) ![Apple MLX](https://img.shields.io/badge/Apple%20MLX-9127C4?style=flat-square&logo=apple&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging%20Face-9127C4?style=flat-square&logo=huggingface&logoColor=white) ![LoRA / 4-bit](https://img.shields.io/badge/LoRA%20%2F%204--bit%20fine--tuning-9127C4?style=flat-square) ![Ollama](https://img.shields.io/badge/Ollama-9127C4?style=flat-square&logo=ollama&logoColor=white) ![OpenAI](https://img.shields.io/badge/OpenAI-9127C4?style=flat-square&logo=openai&logoColor=white) ![Anthropic](https://img.shields.io/badge/Anthropic-9127C4?style=flat-square&logo=anthropic&logoColor=white)

**Systems & Infra** &nbsp;
![Kubernetes](https://img.shields.io/badge/Kubernetes-0A6F8F?style=flat-square&logo=kubernetes&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-0A6F8F?style=flat-square&logo=docker&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0A6F8F?style=flat-square&logo=postgresql&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-0A6F8F?style=flat-square&logo=supabase&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-0A6F8F?style=flat-square&logo=vercel&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-0A6F8F?style=flat-square&logo=nodedotjs&logoColor=white) ![air-gapped / on-prem](https://img.shields.io/badge/air--gapped%20%2F%20on--prem-0A6F8F?style=flat-square) ![SwiftUI](https://img.shields.io/badge/SwiftUI-0A6F8F?style=flat-square&logo=swift&logoColor=white) ![React](https://img.shields.io/badge/React-0A6F8F?style=flat-square&logo=react&logoColor=white) ![Next.js](https://img.shields.io/badge/Next.js-0A6F8F?style=flat-square&logo=nextdotjs&logoColor=white)

**Low-level & Performance** &nbsp;
![NEON SIMD](https://img.shields.io/badge/NEON%20SIMD-955700?style=flat-square) ![Metal GPU kernels](https://img.shields.io/badge/Metal%20GPU%20kernels-955700?style=flat-square&logo=apple&logoColor=white) ![PyO3](https://img.shields.io/badge/PyO3-955700?style=flat-square&logo=rust&logoColor=white) ![COW B-tree](https://img.shields.io/badge/COW%20B--tree-955700?style=flat-square) ![WAL / MVCC](https://img.shields.io/badge/WAL%20%2F%20MVCC-955700?style=flat-square) ![paged KV cache](https://img.shields.io/badge/paged%20KV%20cache-955700?style=flat-square)

**Formal methods & CI** &nbsp;
![TLA+ / TLAPS](https://img.shields.io/badge/TLA%2B%20%2F%20TLAPS-12722B?style=flat-square) ![model checking](https://img.shields.io/badge/model%20checking-12722B?style=flat-square) ![CRDTs](https://img.shields.io/badge/CRDTs-12722B?style=flat-square) ![AES-256](https://img.shields.io/badge/AES--256-12722B?style=flat-square) ![property-based testing](https://img.shields.io/badge/property--based%20testing-12722B?style=flat-square) ![fuzzing](https://img.shields.io/badge/fuzzing-12722B?style=flat-square) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-12722B?style=flat-square&logo=githubactions&logoColor=white)

## 🏆 Awards

- 🥇 **Flinders AI Hackathon** — Top 5 Finalist, of 1,000+ engineers
- 🥉 **Hackbricks by Databricks** — 2nd Runner-Up

## 🎓 About

First principles, then production. I build infrastructure from the ground up — storage engines, inference runtimes, and formally-verified protocols — and ship it to real users. Currently a B.Tech Computer Science student at **Manipal Institute of Technology** (GPA 8.28/10, Aug 2023 – Aug 2027), with research at the Manipal Innovation Cell. My work lives at the intersection of low-level performance, applied AI, and mathematical rigor — NEON kernels and Metal shaders on one end, TLA+ proofs and bootstrap statistics on the other.

## 📫 Let's build something that ships

**[roshan@roshworldwide.com](mailto:roshan@roshworldwide.com)** &nbsp;·&nbsp; [Portfolio](https://roshworldwide.com) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/roshworldwide) &nbsp;·&nbsp; [GitHub](https://github.com/roshworldwide) &nbsp;·&nbsp; Bengaluru, India

<sub>Open to senior & infrastructure roles.</sub>
