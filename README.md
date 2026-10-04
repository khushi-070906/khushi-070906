<img src="assets/banner.svg" width="100%" alt="Khushi Mittal" />

<div align="center">
  <a href="https://github.com/khushi-070906">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2600&pause=800&color=8B5CF6&center=true&vCenter=true&width=800&height=40&lines=I+build+AI+that+helps+people.;Computer+Vision+%7C+RAG+%7C+Agentic+AI;Published+researcher+in+RL;Open-source+contributor+to+kornia-rs;Accepted%3A+Sarvam+%7C+GitLab+%7C+MongoDB" alt="typing" />
  </a>
</div>

<p align="center">
  <a href="https://www.linkedin.com/in/khushi-mittal-7294a2334"><img src="https://img.shields.io/badge/LinkedIn-Connect-8B5CF6?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=161b22" /></a>
  <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7206758"><img src="https://img.shields.io/badge/SSRN-Published-8B5CF6?style=for-the-badge&labelColor=161b22" /></a>
  <a href="mailto:khushimittal070906@gmail.com"><img src="https://img.shields.io/badge/Email-Say%20hi-8B5CF6?style=for-the-badge&logo=gmail&logoColor=white&labelColor=161b22" /></a>
</p>

<img src="assets/ticker.svg" width="100%" alt="" />

<img src="assets/h-short.svg" height="56" alt="whoami" />

<div align="center">
  <img src="assets/terminal.svg" width="85%" alt="terminal intro" />
</div>

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-flows.svg" height="56" alt="projects flowchart" />

### 🧭 The whole map

```mermaid
%%{init: {'theme':'dark','themeVariables':{'primaryColor':'#4A00E0','primaryTextColor':'#ffffff','primaryBorderColor':'#8B5CF6','lineColor':'#C084FC','fontFamily':'monospace'}}}%%
flowchart TB
    K(("Khushi<br/>Mittal")):::core
    K --> R["Research"]
    K --> P["Products"]
    K --> O["Open Source"]
    K --> I["Internships"]
    R --> R1["CGAR - SSRN"]
    P --> P1["DwaniLive"]
    P --> P2["MLflow Drift Plugin"]
    P --> P3["EV Theft Detection"]
    O --> O1["kornia-rs"]
    I --> I1["Zipbolt Innovations"]
    I --> I2["AICTE"]
    I1 -.-> P3
    classDef core fill:#8B5CF6,stroke:#C084FC,color:#fff,stroke-width:3px
    classDef leaf fill:#2563EB,stroke:#60A5FA,color:#fff
    class R1,P1,P2,P3,O1,I1,I2 leaf
```

### 🗣️ DwaniLive: offline live translation + accessible captions
Runs on the presenter's device with **zero internet dependency**. Accepted into the **Sarvam**, **GitLab** and **MongoDB** Startup Programs.

```mermaid
%%{init: {'theme':'dark','themeVariables':{'primaryColor':'#4A00E0','primaryTextColor':'#ffffff','primaryBorderColor':'#8B5CF6','lineColor':'#C084FC','fontFamily':'monospace'}}}%%
flowchart LR
    A(["Presenter speaks"]) --> B["faster-whisper<br/>speech to text"]
    B --> C["NLLB-200<br/>translation"]
    B --> D["FastAPI + WebSockets<br/>asyncio broadcast"]
    C --> D
    D --> E{{"Self-hosted WiFi hotspot<br/>no internet needed"}}
    E --> F["High-contrast live captions<br/>deaf / hard-of-hearing"]
    E --> G["Live spoken translation<br/>blind / visually impaired"]
    style A fill:#8B5CF6,stroke:#C084FC,color:#fff
    style E fill:#2563EB,stroke:#60A5FA,color:#fff
```

### 📉 MLflow Drift Plugin: compliance-mapped drift detection
**31 passing tests.** Maps drift to RBI's draft 2026 Model Risk guidance and DPDP Act Sec. 8(3)-(4), which US tools like Arize and Evidently don't do.

```mermaid
%%{init: {'theme':'dark','themeVariables':{'primaryColor':'#4A00E0','primaryTextColor':'#ffffff','primaryBorderColor':'#8B5CF6','lineColor':'#C084FC','fontFamily':'monospace'}}}%%
flowchart LR
    A["Model + feature data"] --> C["detector"]
    B["baseline"] --> C
    G["config"] --> C
    C --> D["Airflow / MLflow hooks"]
    D --> E["reporting"]
    C --> F{{"Compliance layer"}}
    F --> H["RBI draft 2026<br/>Model Risk guidance"]
    F --> I["DPDP Act<br/>Sec. 8(3)-(4)"]
    F --> E
    style F fill:#8B5CF6,stroke:#C084FC,color:#fff
```

### 🚗 EV Theft Detection: Raspberry Pi security
Built during my research internship at Zipbolt Innovations.

```mermaid
%%{init: {'theme':'dark','themeVariables':{'primaryColor':'#4A00E0','primaryTextColor':'#ffffff','primaryBorderColor':'#8B5CF6','lineColor':'#C084FC','fontFamily':'monospace'}}}%%
flowchart LR
    A["Onboard sensors"] -->|"unauthorized movement<br/>or tampering"| B["Raspberry Pi"]
    B --> C["Camera"]
    C --> D[("Recorded theft attempt")]
    style B fill:#8B5CF6,stroke:#C084FC,color:#fff
    style D fill:#2563EB,stroke:#60A5FA,color:#fff
```

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-research.svg" height="56" alt="research" />

**CGAR: Confidence-Gated Adaptive Routing for RL-Based API Gateways** · [📄 SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7206758)

```mermaid
%%{init: {'theme':'dark','themeVariables':{'primaryColor':'#4A00E0','primaryTextColor':'#ffffff','primaryBorderColor':'#8B5CF6','lineColor':'#C084FC','fontFamily':'monospace'}}}%%
flowchart LR
    A["API requests"] --> B["Gateway routing<br/>under autoscaling"]
    B --> C["Non-stationary<br/>per-arm warm-start bandit"]
    C --> D{{"Confidence gate<br/>(CGAR)"}}
    D --> E["Routing decision"]
    E --> F["81.6 to 91.9% regret reduction<br/>7 baselines, 20 seeds"]
    style D fill:#8B5CF6,stroke:#C084FC,color:#fff
    style F fill:#2563EB,stroke:#60A5FA,color:#fff
```

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-oss.svg" height="56" alt="open source" />

**[kornia-rs](https://github.com/kornia/kornia-rs)**: computer vision in Rust, with Python bindings

```mermaid
%%{init: {'theme':'dark','themeVariables':{'primaryColor':'#4A00E0','primaryTextColor':'#ffffff','primaryBorderColor':'#8B5CF6','lineColor':'#C084FC','fontFamily':'monospace'}}}%%
flowchart LR
    K(("kornia-rs")):::core
    K --> A["Doctest discovery gap<br/>docstrings silently skipped"] --> A2["Fixed: recursive<br/>test collection"]
    K --> B["Aliasing UB in<br/>fused ColorJitter path"] --> B2["Resolved"]
    K --> C["Panics on<br/>malformed inputs"] --> C2["Proper Python<br/>exceptions"]
    classDef core fill:#8B5CF6,stroke:#C084FC,color:#fff,stroke-width:3px
    style A2 fill:#2563EB,stroke:#60A5FA,color:#fff
    style B2 fill:#2563EB,stroke:#60A5FA,color:#fff
    style C2 fill:#2563EB,stroke:#60A5FA,color:#fff
```

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-arsenal.svg" height="56" alt="arsenal" />

<div align="center">
  <img src="assets/orbit.svg" width="80%" alt="skills orbit" />
  <br/>
  <img src="https://skillicons.dev/icons?i=python,c,cpp,java,mysql,pytorch,tensorflow,sklearn,opencv,fastapi,azure,git,github,figma,rust&theme=dark" />
</div>

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-proof.svg" height="56" alt="proof of work" />

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=khushi-070906&show_icons=true&hide_border=true&bg_color=0d1117&title_color=A855F7&icon_color=3B82F6&text_color=8b949e&count_private=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=khushi-070906&layout=compact&hide_border=true&bg_color=0d1117&title_color=A855F7&text_color=8b949e" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=khushi-070906&hide_border=true&background=0d1117&stroke=8b5cf6&ring=A855F7&fire=3B82F6&currStreakLabel=A855F7&sideLabels=8b949e&dates=6b7280&currStreakNum=e6edf3&sideNums=e6edf3" />
</div>

<br/>

<div align="center">
  <img width="100%" src="profile-3d-contrib/profile-night-rainbow.svg" alt="3D contribution graph" />
</div>

<br/>

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/khushi-070906/khushi-070906/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/khushi-070906/khushi-070906/output/github-snake.svg" />
    <img alt="snake eating my contributions" width="100%" src="https://raw.githubusercontent.com/khushi-070906/khushi-070906/output/github-snake-dark.svg" />
  </picture>
</div>

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-wins.svg" height="56" alt="wins" />

| | |
| :-- | :-- |
| 🥇 **Rank 1, Perfect 100** | ICTRD Data Science Program (2025) |
| 🎨 **Winner** | Ctrl+Alt+Design, IEEE DTU x IEEE GTBIT (2025) |
| 🚀 **Accepted** | Sarvam, GitLab and MongoDB Startup Programs |
| 📖 **Published** | CGAR on SSRN |

<div align="center">
<br/>
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=17&duration=3000&pause=1000&color=8B5CF6&center=true&vCenter=true&width=520&lines=Thanks+for+stopping+by.;Now+go+build+something." alt="footer" />
</div>

<img src="assets/banner.svg" width="100%" alt="" />
