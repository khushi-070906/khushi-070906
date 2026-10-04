<img src="assets/banner.svg" width="100%" alt="Khushi Mittal" />

<div align="center">
  <a href="https://github.com/khushi-070906">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2600&pause=800&color=8B5CF6&center=true&vCenter=true&width=800&height=40&lines=I+build+AI+that+helps+people.;Computer+Vision+%7C+RAG+%7C+Agentic+AI;Published+researcher+in+RL;Open-source+contributor+to+kornia-rs;Patent-pending+assistive+tech." alt="typing" />
  </a>
</div>

<p align="center">
  <a href="https://www.linkedin.com/in/khushi-mittal-7294a2334"><img src="https://img.shields.io/badge/LinkedIn-Connect-8B5CF6?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=161b22" /></a>
  <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7206758"><img src="https://img.shields.io/badge/SSRN-Published-8B5CF6?style=for-the-badge&labelColor=161b22" /></a>
  <a href="mailto:khushimittal070906@gmail.com"><img src="https://img.shields.io/badge/Email-Say%20hi-8B5CF6?style=for-the-badge&logo=gmail&logoColor=white&labelColor=161b22" /></a>
</p>

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-short.svg" height="56" alt="whoami" />

<div align="center">
  <img src="assets/terminal.svg" width="85%" alt="terminal intro" />
</div>

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-building.svg" height="56" alt="building" />

### 👁️ V2T-Graph / VisionSense — *Patent Pending*
A monocular camera becomes a navigation aid for visually impaired users. Part of **SmartSight**, an AI + IIoT platform (ESP32 sensors, bone-conduction audio, multilingual voice, OCR, SOS alerts).

```mermaid
flowchart LR
    A([Monocular camera]) --> B[YOLOv10<br/>object detection]
    A --> C[Depth Anything V2<br/>depth estimation]
    B --> D{{Scene graph}}
    C --> D
    D --> E[Heading-based<br/>pruning]
    E --> F([Tactile + audio cues])
    style A fill:#4A00E0,color:#fff,stroke:#8B5CF6
    style D fill:#8B5CF6,color:#fff,stroke:#C084FC
    style F fill:#3B82F6,color:#fff,stroke:#60A5FA
```

<details>
<summary><b>🗣️ DwaniLive</b>: offline live speech translation + accessible captioning</summary>
<br/>

Runs on the presenter's device and broadcasts over a self-hosted WiFi hotspot with **zero internet dependency**. Real-time high-contrast captions for deaf and hard-of-hearing attendees, live spoken translation for blind and visually impaired attendees.

`Python` `FastAPI` `faster-whisper` `NLLB-200` `WebSockets` `asyncio`

🚀 Accepted into the **Sarvam**, **GitLab** and **MongoDB** Startup Programs.
</details>

<details>
<summary><b>📉 MLflow Drift Plugin</b>: compliance-mapped drift detection</summary>
<br/>

MLflow/Airflow plugin for model and feature drift (detector, baseline, config, hooks, reporting), backed by **31 passing tests**. Maps drift to **RBI's draft 2026 Model Risk guidance** and **DPDP Act Sec. 8(3)-(4)**, which US tools like Arize and Evidently don't do.

`Python` `MLflow` `Airflow`
</details>

<details>
<summary><b>🚗 EV Theft Detection</b>: Raspberry Pi security system</summary>
<br/>

Camera records theft attempts while onboard sensors detect unauthorized movement and tampering. Built during my research internship at Zipbolt Innovations.
</details>

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-research.svg" height="56" alt="research" />

**CGAR: Confidence-Gated Adaptive Routing for RL-Based API Gateways** · [📄 SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7206758)

| Problem | Approach | Result |
| :--- | :--- | :--- |
| API gateway routing under autoscaling is non-stationary | Modeled as a per-arm warm-start bandit with a confidence-gated RL framework | **81.6 to 91.9% regret reduction** across 7 baselines, 20 seeds |

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-oss.svg" height="56" alt="open source" />

**[kornia-rs](https://github.com/kornia/kornia-rs)**: computer vision in Rust, with Python bindings

- 🐛 Fixed a doctest-discovery gap where docstrings were silently skipped in recursive test collection
- 🧨 Resolved an aliasing UB bug in the fused `ColorJitter` path
- 🛡️ Replaced panics with proper Python exceptions for malformed inputs

<img src="assets/divider.svg" width="100%" alt="" />

<img src="assets/h-arsenal.svg" height="56" alt="arsenal" />

<div align="center">
<br/>

<img src="https://skillicons.dev/icons?i=python,c,cpp,java,mysql,pytorch,tensorflow,sklearn&theme=dark" />
<br/>
<img src="https://skillicons.dev/icons?i=opencv,fastapi,azure,git,github,figma,rust&theme=dark" />

<br/><br/>

<img src="https://img.shields.io/badge/LangChain-8B5CF6?style=flat-square&logo=langchain&logoColor=white&labelColor=161b22" />
<img src="https://img.shields.io/badge/LangGraph-8B5CF6?style=flat-square&labelColor=161b22" />
<img src="https://img.shields.io/badge/RAG-8B5CF6?style=flat-square&labelColor=161b22" />
<img src="https://img.shields.io/badge/Multi--Agent-8B5CF6?style=flat-square&labelColor=161b22" />
<img src="https://img.shields.io/badge/HuggingFace-8B5CF6?style=flat-square&logo=huggingface&logoColor=white&labelColor=161b22" />
<img src="https://img.shields.io/badge/BERT-8B5CF6?style=flat-square&labelColor=161b22" />
<img src="https://img.shields.io/badge/Whisper-8B5CF6?style=flat-square&labelColor=161b22" />
<img src="https://img.shields.io/badge/Keras-8B5CF6?style=flat-square&logo=keras&logoColor=white&labelColor=161b22" />
<img src="https://img.shields.io/badge/Streamlit-8B5CF6?style=flat-square&logo=streamlit&logoColor=white&labelColor=161b22" />
<img src="https://img.shields.io/badge/MLflow-8B5CF6?style=flat-square&logo=mlflow&logoColor=white&labelColor=161b22" />
<img src="https://img.shields.io/badge/Airflow-8B5CF6?style=flat-square&logo=apacheairflow&logoColor=white&labelColor=161b22" />

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
| 📜 **Patent pending** | V2T-Graph |
| 📖 **Published** | CGAR on SSRN |

<div align="center">
<br/>
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=17&duration=3000&pause=1000&color=8B5CF6&center=true&vCenter=true&width=520&lines=Thanks+for+stopping+by.;Now+go+build+something." alt="footer" />
</div>

<img src="assets/banner.svg" width="100%" alt="" />
