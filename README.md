<img src="assets/banner.svg" width="100%" alt="Khushi Mittal" />

<div align="center">
  <a href="https://github.com/khushi-070906">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2600&pause=800&color=0E9AA7&center=true&vCenter=true&width=800&height=40&lines=I+build+AI+that+helps+people.;Computer+Vision+%7C+RAG+%7C+Agentic+AI;Published+researcher+in+RL;Built+the+backend+for+RAVS;Open-source+contributor+to+kornia-rs;Accepted%3A+Sarvam+%7C+GitLab+%7C+MongoDB" alt="typing" />
  </a>
</div>

<p align="center">
  <a href="https://www.linkedin.com/in/khushi-mittal-7294a2334"><img src="https://img.shields.io/badge/LinkedIn-Connect-0E9AA7?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0B3C49" /></a>
  <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7206758"><img src="https://img.shields.io/badge/SSRN-Published-F2705E?style=for-the-badge&labelColor=0B3C49" /></a>
  <a href="mailto:khushimittal070906@gmail.com"><img src="https://img.shields.io/badge/Email-Say%20hi-0E9AA7?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0B3C49" /></a>
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
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#CFF3EE','primaryTextColor':'#0B3C49','primaryBorderColor':'#0E9AA7','lineColor':'#0E9AA7','secondaryColor':'#FFE8C2','tertiaryColor':'#FFF6E5','fontFamily':'monospace'}}}%%
flowchart TB
    K(("Khushi<br/>Mittal")):::core
    K --> R["Research"]
    K --> P["Products"]
    K --> O["Open Source"]
    K --> I["Internships"]
    R --> R1["CGAR - SSRN"]
    P --> P1["DwaniLive"]
    P --> P2["RAVS backend"]
    O --> O1["kornia-rs"]
    I --> I1["Zipbolt Innovations"]
    I --> I2["AICTE"]
    classDef core fill:#FFB4A8,stroke:#F2705E,color:#0B3C49,stroke-width:3px
    classDef leaf fill:#BAE6FD,stroke:#0369A1,color:#0B3C49
    class R1,P1,P2,O1,I1,I2 leaf
```

### 🎓 RAVS (Research Connect): I built the backend
A role-based **research attendance and verification** app. Students authenticate, check in and out of lab sessions and submit work evidence. Faculty review those sessions before approved hours count toward attendance reports. Admins manage users and lab configuration. Also covers presence checks, events, leave, certificates and a live roster. **Supabase** provides auth, database and storage.

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#CFF3EE','primaryTextColor':'#0B3C49','primaryBorderColor':'#0E9AA7','lineColor':'#0E9AA7','secondaryColor':'#FFE8C2','tertiaryColor':'#FFF6E5','fontFamily':'monospace'}}}%%
flowchart TB
    subgraph STU["Student"]
        direction LR
        s1["Sign in"] --> s2["Check in<br/>with lab code"] --> s3["Presence checks"] --> s4["Log work evidence<br/>+ session timer"] --> s5["Check out"]
    end
    subgraph FAC["Faculty"]
        direction LR
        f1["Review sessions<br/>+ time corrections"] --> f2["Approve hours"] --> f3["Attendance reports<br/>+ research summaries"]
    end
    subgraph OPS["Lab operations"]
        direction LR
        o1["Live roster"]
        o2["Events + calendar"]
        o3["Leave requests"]
        o4["Certificates +<br/>verification codes"]
    end
    subgraph ADM["Head admin"]
        a1["Manage users + labs"]
    end
    STU --> DB
    FAC --> DB
    OPS --> DB
    ADM --> DB
    DB[("Supabase<br/>auth + database + storage")]
    style DB fill:#FFB4A8,stroke:#F2705E,color:#0B3C49,stroke-width:2px
    style f2 fill:#FFE8C2,stroke:#F2705E,color:#0B3C49
```

### 🗣️ DwaniLive: offline live translation + accessible captions
Runs on the presenter's device with **zero internet dependency**. Accepted into the **Sarvam**, **GitLab** and **MongoDB** Startup Programs.

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#CFF3EE','primaryTextColor':'#0B3C49','primaryBorderColor':'#0E9AA7','lineColor':'#0E9AA7','secondaryColor':'#FFE8C2','tertiaryColor':'#FFF6E5','fontFamily':'monospace'}}}%%
flowchart LR
    A(["Presenter speaks"]) --> B["faster-whisper<br/>speech to text"]
    B --> C["NLLB-200<br/>translation"]
    B --> D["FastAPI + WebSockets<br/>asyncio broadcast"]
    C --> D
    D --> E{{"Self-hosted WiFi hotspot<br/>no internet needed"}}
    E --> F["High-contrast live captions<br/>deaf / hard-of-hearing"]
    E --> G["Live spoken translation<br/>blind / visually impaired"]
    style A fill:#FFB4A8,stroke:#F2705E,color:#0B3C49
    style E fill:#BAE6FD,stroke:#0369A1,color:#0B3C49
```

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-research.svg" height="56" alt="research" />

**CGAR: Confidence-Gated Adaptive Routing for RL-Based API Gateways** · [📄 SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7206758)

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#CFF3EE','primaryTextColor':'#0B3C49','primaryBorderColor':'#0E9AA7','lineColor':'#0E9AA7','secondaryColor':'#FFE8C2','tertiaryColor':'#FFF6E5','fontFamily':'monospace'}}}%%
flowchart LR
    A["API requests"] --> B["Gateway routing<br/>under autoscaling"]
    B --> C["Non-stationary<br/>per-arm warm-start bandit"]
    C --> D{{"Confidence gate<br/>(CGAR)"}}
    D --> E["Routing decision"]
    E --> F["81.6 to 91.9% regret reduction<br/>7 baselines, 20 seeds"]
    style D fill:#FFB4A8,stroke:#F2705E,color:#0B3C49
    style F fill:#BAE6FD,stroke:#0369A1,color:#0B3C49
```

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-oss.svg" height="56" alt="open source" />

**[kornia-rs](https://github.com/kornia/kornia-rs)**: computer vision in Rust, with Python bindings

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#CFF3EE','primaryTextColor':'#0B3C49','primaryBorderColor':'#0E9AA7','lineColor':'#0E9AA7','secondaryColor':'#FFE8C2','tertiaryColor':'#FFF6E5','fontFamily':'monospace'}}}%%
flowchart LR
    K(("kornia-rs")):::core
    K --> A["Doctest discovery gap<br/>docstrings silently skipped"] --> A2["Fixed: recursive<br/>test collection"]
    K --> B["Aliasing UB in<br/>fused ColorJitter path"] --> B2["Resolved"]
    K --> C["Panics on<br/>malformed inputs"] --> C2["Proper Python<br/>exceptions"]
    classDef core fill:#FFB4A8,stroke:#F2705E,color:#0B3C49,stroke-width:3px
    style A2 fill:#BAE6FD,stroke:#0369A1,color:#0B3C49
    style B2 fill:#BAE6FD,stroke:#0369A1,color:#0B3C49
    style C2 fill:#BAE6FD,stroke:#0369A1,color:#0B3C49
```

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-arsenal.svg" height="56" alt="arsenal" />

<div align="center">
  <img src="assets/orbit.svg" width="80%" alt="skills orbit" />
  <br/>
  <img src="https://skillicons.dev/icons?i=python,c,cpp,java,mysql,pytorch,tensorflow,sklearn,opencv,fastapi,azure,supabase,ts,git,github,figma,rust&theme=light" />
</div>

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-proof.svg" height="56" alt="proof of work" />

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=khushi-070906&show_icons=true&hide_border=true&bg_color=FFF6E5&title_color=0E7490&icon_color=F2705E&text_color=0B3C49&count_private=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=khushi-070906&layout=compact&hide_border=true&bg_color=FFF6E5&title_color=0E7490&text_color=0B3C49" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=khushi-070906&hide_border=true&background=FFF6E5&stroke=0E9AA7&ring=F2705E&fire=FBBF24&currStreakLabel=0E7490&sideLabels=0B3C49&dates=64748b&currStreakNum=0B3C49&sideNums=0B3C49" />
</div>

<br/>

<div align="center">
  <img width="100%" src="profile-3d-contrib/profile-green-animate.svg" alt="3D contribution graph" />
</div>

<br/>

<div align="center">
  <img width="100%" alt="snake eating my contributions" src="https://raw.githubusercontent.com/khushi-070906/khushi-070906/output/snake-ocean.svg" />
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
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=17&duration=3000&pause=1000&color=0E9AA7&center=true&vCenter=true&width=520&lines=Thanks+for+stopping+by.;Now+go+build+something." alt="footer" />
</div>

<img src="assets/footer.svg" width="100%" alt="" />
