<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0D1117,50:15315B,100:1F6FEB&height=140&section=header&text=Dwij%20Desai&fontSize=44&fontColor=FFFFFF&fontAlignY=42&desc=Backend%20%C2%B7%20Applied%20AI%20%C2%B7%20Retrieval%20Systems&descAlignY=68&descSize=15" width="100%" alt="Dwij Desai — Backend, Applied AI, Retrieval Systems" />

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=19&duration=3200&pause=900&color=1F6FEB&center=true&vCenter=true&width=620&height=40&lines=Final-year+Computer+Science+%26+Engineering;I+build+backend+services+and+retrieval+systems;Available+full-time+from+January+2027" alt="Backend and applied AI engineering" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dwij-desai-797644276/)
[![Email](https://img.shields.io/badge/Email-1F6FEB?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dwijdvd@gmail.com)

</div>

---

I build backend and applied-AI systems in Python — mostly at the point where retrieval, APIs and deployment meet. My current focus is making language-model output **traceable**: answers that can be tied back to the exact source text that produced them, rather than trusted on faith.

**B.Tech, Computer Science and Engineering** — Specialization: Big Data Analysis
Ganpat University, Institute of Computer Technology · 2023–2027 · currently 7th semester

<br/>

## Featured — Retrieval-Aware Chat Engine

> A retrieval-augmented generation backend, built as a running service rather than a notebook.

<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI" />
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain" />
<img src="https://img.shields.io/badge/ChromaDB-FF6B4A?style=flat-square" alt="ChromaDB" />
<img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" alt="Pytest" />
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
</p>

**How one request flows through it**

```mermaid
flowchart LR
    A(["Client"]) --> B["FastAPI /ask"]
    B --> C["Load chat history<br/>SQLite"]
    C --> D["Retrieve top-k chunks<br/>ChromaDB"]
    D --> E["Assemble grounded prompt"]
    E --> F{"Primary LLM"}
    F -- success --> G["Answer + source metadata"]
    F -- "quota / transient" --> H["Fallback model"]
    H --> G
    G --> I(["Persist turn · return"])

    style F fill:#1F6FEB,stroke:#1F6FEB,color:#fff
    style G fill:#15315B,stroke:#1F6FEB,color:#fff
```

|  | |
|:--|:--|
| **Ingestion** | Five document formats — PDF, TXT, CSV, XLSX, JSON — recursively chunked into a persistent vector store |
| **Embeddings** | `bge-small-en-v1.5` runs locally; document content never leaves the machine during indexing |
| **Resilience** | Provider abstraction across two LLM backends with error-classified fallback — quota and transient upstream failures retry against a secondary model, while malformed input and auth errors fail fast |
| **Memory** | Persistent multi-turn history in SQLite, loaded *before* retrieval so follow-up questions resolve against recent context |
| **Traceability** | Every retrieved chunk carries its source file and record index, so an answer can be tied to the text behind it |
| **Operations** | Multi-stage container build · pytest suite over ingestion behaviour and RAG-engine contracts · LangSmith tracing |

<a href="https://github.com/Dwij-desai/Retrieval-Aware-Chat-Engine">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=Dwij-desai&repo=Retrieval-Aware-Chat-Engine&bg_color=00000000&title_color=1F6FEB&text_color=808A96&icon_color=1F6FEB&border_color=30363D&show_owner=false" alt="Retrieval-Aware Chat Engine repository" />
</a>

<sub>The repository README states component status explicitly — what is implemented, what is documented, and what I have personally validated are three different things, and it distinguishes them.</sub>

<br/>

## Other projects

<p>
<a href="https://github.com/Dwij-desai/Online-Compiler">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=Dwij-desai&repo=Online-Compiler&bg_color=00000000&title_color=1F6FEB&text_color=808A96&icon_color=1F6FEB&border_color=30363D&show_owner=false" alt="Online Compiler Platform" />
</a>
<a href="https://github.com/Dwij-desai/AI_Course_Recommender">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=Dwij-desai&repo=AI_Course_Recommender&bg_color=00000000&title_color=1F6FEB&text_color=808A96&icon_color=1F6FEB&border_color=30363D&show_owner=false" alt="AI Course Recommender" />
</a>
</p>

**Online Compiler Platform** — browser-based interface for compiling and running code, with execution isolated in containers. `React.js` `Docker` `REST API`

**Course Recommendation System** — similarity-based recommender; built the preprocessing pipeline and evaluated model performance. `Python` `Pandas` `scikit-learn`

<br/>

## Experience

**Software Engineering Intern** — Biz App Dev · Jan – Jun 2024 *(6 months)*
Developed backend modules and REST API endpoints used by internal teams. Debugged and refactored application code to improve stability.

<br/>

## Toolkit

**Working knowledge** — what I've built with

<img src="https://skillicons.dev/icons?i=python,fastapi,docker,sqlite,git,linux,react,ts,vite,github&theme=dark" alt="Python, FastAPI, Docker, SQLite, Git, Linux, React, TypeScript, Vite, GitHub" />

<details>
<summary><b>Coursework and exposure</b> — smaller exercises, not work I'd claim production experience in</summary>

<br/>

`C++` · `Java` · `JavaScript` · `Angular` · `scikit-learn` · `PyTorch` · `Pandas` · `Hadoop` · `Apache Spark` · `MySQL`

Two tiers on purpose. I'd rather you trust the first list than wonder about the second.

</details>

<details>
<summary><b>Certifications</b></summary>

<br/>

- Machine Learning Specialization — Andrew Ng, Coursera *(2025)*
- Python for Data Science — NPTEL *(2025)*
- Docker Essentials — LinkedIn Learning *(2025)*
- SQL Essential Training — LinkedIn Learning *(2024)*
- CCNA: Routing and Switching Essentials — Cisco *(2024)*

</details>

<br/>

<div align="center">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Dwij-desai&layout=compact&langs_count=8&bg_color=00000000&title_color=1F6FEB&text_color=808A96&border_color=30363D&hide=jupyter%20notebook" alt="Most used languages" />
</div>

<br/>

---

<div align="center">

### Available full-time from January 2027

Looking for a **4–6 month software / backend / applied-AI internship**.

[![Email](https://img.shields.io/badge/dwijdvd@gmail.com-1F6FEB?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dwijdvd@gmail.com)
[![LinkedIn](https://img.shields.io/badge/Connect%20on%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dwij-desai-797644276/)

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:1F6FEB,50:15315B,100:0D1117&height=60&section=footer" width="100%" alt="" />
