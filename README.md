# Dwij Desai

Final-year Computer Science & Engineering student. I build backend and applied-AI systems in
Python — mostly at the point where retrieval, APIs and deployment meet.

Looking for a software / backend / applied-AI internship from January 2027.

---

### Education

**B.Tech, Computer Science and Engineering** — Specialization: Big Data Analysis  
Ganpat University, Institute of Computer Technology · 2023–2027 · currently 7th semester

---

### Focus areas

- **Backend engineering** — FastAPI services, REST API design, containerised deployment
- **Retrieval-augmented generation** — ingestion pipelines, chunking, embeddings, vector search, context-grounded generation
- **Applied AI integration** — provider abstraction, fallback routing, tracing, evaluation scaffolding
- **Data handling** — SQL, Pandas, multi-format ingestion (PDF, TXT, CSV, XLSX, JSON)

---

### Selected projects

#### [Retrieval-Aware Chat Engine](https://github.com/Dwij-desai/Retrieval-Aware-Chat-Engine)
*A RAG backend built as a service rather than a notebook.*  
`FastAPI` `LangChain` `ChromaDB` `HuggingFace embeddings` `SQLite` `Docker` `Pytest` `React + TypeScript`

- Multi-format ingestion (PDF / TXT / CSV / XLSX / JSON) with recursive chunking into a persistent vector store
- Local embeddings via `bge-small-en-v1.5` — document content never leaves the machine during indexing
- Provider abstraction across Groq and Google Gemini, with error-classified fallback: quota, model-unavailable and transient upstream failures retry against a secondary model; malformed input and auth errors fail fast
- Persistent multi-turn conversation memory in SQLite, loaded before retrieval so follow-up questions resolve against recent context
- Each retrieved chunk carries its source file and row/item index, so an answer can be traced back to the text that produced it
- Containerised deployment; pytest suite covering ingestion behaviour and RAG-engine contracts

The README states component status explicitly — what is implemented, what is documented, and what
I have personally validated are three different things, and it distinguishes them.

#### [Online Compiler Platform](https://github.com/Dwij-desai/Online-Compiler)
*Browser-based code execution with containerised isolation.*  
`React.js` `Docker` `REST API`

- Web interface for compiling and running code, with execution isolated in containers

#### [Course Recommendation System](https://github.com/Dwij-desai/AI_Course_Recommender)
*Similarity-based course recommender.*  
`Python` `Pandas` `scikit-learn`

- Data preprocessing pipeline and model evaluation over course metadata

---

### Experience

**Software Engineering Intern** — Biz App Dev · Jan – Jun 2024  
Backend modules and REST API endpoints used by internal teams. Debugging and refactoring
work on application stability.

---

### Technical skills

| | |
|---|---|
| **Working knowledge** | Python · FastAPI · REST APIs · SQL / SQLite · Docker · Git · Linux · React · Pandas |
| **Coursework / exposure** | C++ · Java · JavaScript · scikit-learn · PyTorch · Hadoop · Apache Spark |

Two tiers on purpose. The second row is coursework and small exercises, not work I would claim
production experience in.

---

### Contact

dwijdvd@gmail.com · [LinkedIn](https://www.linkedin.com/in/dwij-desai-797644276/)