<div align="center">

<h1>Dwij Desai</h1>

<p><strong>Backend · Applied AI · Retrieval Systems</strong></p>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=16&duration=3200&pause=900&color=1F6FEB&center=true&vCenter=true&width=330&height=30&lines=Final-year+CS+%26+Engineering;I+build+backend+%26+retrieval+systems;Free+full-time+from+January+2027" alt="Final-year CS and Engineering. I build backend and retrieval systems. Free full-time from January 2027." />

<p>
<a href="https://www.linkedin.com/in/dwij-desai-797644276/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:dwijdvd@gmail.com"><img src="https://img.shields.io/badge/Email-1F6FEB?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

</div>

---

I build backend and applied-AI systems in Python, where retrieval, APIs and deployment meet.

My focus is making language-model output **traceable** — answers you can tie back to the exact source text that produced them, rather than trust on faith.

<strong>B.Tech, Computer Science and Engineering</strong><br>
Specialization: Big Data Analysis<br>
Ganpat University · 2023–2027 · 7th semester

<br>

## Retrieval-Aware Chat Engine

A retrieval-augmented generation backend, built as a running service rather than a notebook.

<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI" />
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain" />
<img src="https://img.shields.io/badge/ChromaDB-FF6B4A?style=flat-square" alt="ChromaDB" />
<img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
</p>

<img src="architecture.svg" width="100%" alt="Request flow: FastAPI validation, load conversation memory from SQLite, retrieve top-k chunks from ChromaDB, assemble a grounded prompt, call the primary LLM with a fallback model on retryable errors, return the answer with its source chunks, persist the turn." />

**What it does**

- **Ingests five formats** — PDF, TXT, CSV, XLSX, JSON — chunked into a persistent vector store
- **Embeds locally** with `bge-small-en-v1.5`, so document content never leaves the machine during indexing
- **Survives provider failure** — one abstraction layer over two LLM backends; quota and transient errors retry on a secondary model, while bad input and auth errors fail fast
- **Remembers the conversation** in SQLite, loaded *before* retrieval so follow-ups resolve against recent context
- **Stays traceable** — every chunk carries its source file and record index

<p>
<a href="https://github.com/Dwij-desai/Retrieval-Aware-Chat-Engine"><img src="https://img.shields.io/badge/View%20the%20repository-1F6FEB?style=for-the-badge&logo=github&logoColor=white" alt="View the repository" /></a>
</p>

<sub>Its README separates what is implemented, what is documented, and what I have personally validated.</sub>

<br>

## Other projects

<strong>Online Compiler Platform</strong><br>
Browser-based interface for compiling and running code, with execution isolated in containers.

<p>
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/REST%20API-6E7681?style=flat-square" alt="REST API" />
<a href="https://github.com/Dwij-desai/Online-Compiler"><img src="https://img.shields.io/badge/Repo-238636?style=flat-square&logo=github&logoColor=white" alt="Repository" /></a>
</p>

<strong>Course Recommendation System</strong><br>
Similarity-based recommender — built the preprocessing pipeline and evaluated model performance.

<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="Pandas" />
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white" alt="scikit-learn" />
<a href="https://github.com/Dwij-desai/AI_Course_Recommender"><img src="https://img.shields.io/badge/Repo-238636?style=flat-square&logo=github&logoColor=white" alt="Repository" /></a>
</p>

<br>

## Experience

<strong>Software Engineering Intern</strong> — Biz App Dev<br>
<em>Jan – Jun 2024 · 6 months</em>

Built backend modules and REST API endpoints used by internal teams. Debugged and refactored application code to improve stability.

<br>

## Toolkit

Tools I've actually built with:

<p>
<img src="https://skillicons.dev/icons?i=python,fastapi,docker,sqlite,git&theme=dark" alt="Python, FastAPI, Docker, SQLite, Git" />
</p>
<p>
<img src="https://skillicons.dev/icons?i=linux,react,ts,vite,github&theme=dark" alt="Linux, React, TypeScript, Vite, GitHub" />
</p>

<details>
<summary><strong>Coursework and exposure</strong></summary>
<br>
<p><code>C++</code> · <code>Java</code> · <code>JavaScript</code> · <code>Angular</code> · <code>scikit-learn</code> · <code>PyTorch</code> · <code>Pandas</code> · <code>Hadoop</code> · <code>Apache Spark</code> · <code>MySQL</code></p>
<p>Two tiers on purpose — I'd rather you trust the icons above than wonder about this list.</p>
</details>

<details>
<summary><strong>Certifications</strong></summary>
<br>
<ul>
<li>Machine Learning Specialization — Andrew Ng, Coursera <em>(2025)</em></li>
<li>Python for Data Science — NPTEL <em>(2025)</em></li>
<li>Docker Essentials — LinkedIn Learning <em>(2025)</em></li>
<li>SQL Essential Training — LinkedIn Learning <em>(2024)</em></li>
<li>CCNA: Routing and Switching Essentials — Cisco <em>(2024)</em></li>
</ul>
</details>

---

<div align="center">

<h3>Available from January 2027</h3>

<p>Looking for a <strong>4–6 month backend / applied-AI internship</strong></p>

<p>
<a href="mailto:dwijdvd@gmail.com"><img src="https://img.shields.io/badge/Get%20in%20touch-1F6FEB?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://www.linkedin.com/in/dwij-desai-797644276/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
</p>

</div>
