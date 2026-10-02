<div align="center">

# Hi, I'm Samavi Nasir 👋

### AI Engineer | Agentic AI · LLM Applications · Data Engineering

I build AI-powered applications, agentic workflows, and data-driven systems, from model development and orchestration to APIs, databases, and deployment.

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3000&pause=1000&color=3B82F6&center=true&vCenter=true&width=850&lines=Building+Agentic+AI+Systems;Engineering+LLM-Powered+Applications;Designing+Reliable+AI+Workflows;From+Machine+Learning+to+Production;AI+Engineering+%7C+Data+Engineering"/>

<br>

<a href="https://samavinasir.vercel.app/ai"><img src="https://img.shields.io/badge/Portfolio-2563EB?style=for-the-badge&logo=vercel&logoColor=white"/></a>
<a href="https://linkedin.com/in/samavinasir"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:samavi.nasir96@gmail.com"><img src="https://img.shields.io/badge/Email-0EA5A4?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://scholar.google.com/citations?user=K_okdSMAAAAJ&hl=en"><img src="https://img.shields.io/badge/Google%20Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white"/></a>

<br><br>

<img src="https://komarev.com/ghpvc/?username=samavinasir&label=Profile%20Views&color=2563EB&style=flat-square"/>

</div>

---

## 👨‍💻 About Me

I'm an **AI Engineer** focused on building intelligent applications that solve practical problems using machine learning, large language models, agent orchestration, and data engineering.

My experience spans the AI development lifecycle, from data processing and model development to backend engineering, API integration, database design, and deployment on Linux-based infrastructure.

I enjoy turning complex requirements into working software, integrating specialized tools into coherent workflows, and building systems that are useful, inspectable, and maintainable.

My background includes applied machine learning and scientific computing, where I have developed AI models and software for complex research problems. I bring that experience into broader AI engineering applications, including agentic systems, LLM-powered tools, and research automation.

### 🎯 Current Focus

* 🤖 Agentic AI and multi-agent orchestration
* 🧠 LLM applications, RAG, and tool-using agents
* 🔗 LangGraph, LangChain, and workflow design
* ⚙️ Backend engineering and AI-powered APIs
* 🗄️ Data engineering, PostgreSQL, and vector databases
* 🐳 Docker, CI/CD, and production-oriented deployment
* 📊 Machine learning, model evaluation, and MLOps
* ⚡ Apache Spark and distributed data processing

---

## 🚀 Featured Projects

### 🔎 TraceReview | Literature review you can trace

> Ask a research question and get a focused set of relevant papers as source-checked reading cards, with every step of the workflow inspectable.

<!-- TODO: add a screenshot, e.g. <img src="docs/screenshot.png" width="800"/> -->

**Problem:** Researchers need help finding and reading relevant papers.

**What I built:** TraceReview is a literature-review assistant built as a controlled LangGraph workflow. It searches scholarly sources, selects up to 10 papers, and turns available records into reading cards with bibliographic details, an AI-generated study summary, source-matched excerpts, and the abstract’s final sentence copied from the record. Researchers interpret the papers; TraceReview does not decide whether their findings are true.

**Engineering highlights**
 
* **Source-first design:** The app presents paper-level reading aids and source wording so researchers can assess the evidence themselves.
* **Checked excerpts:** The app checks proposed quotes against the abstract, and falls back to relevant abstract sentences copied verbatim when needed.
* **Focused retrieval:** PubMed and Europe PMC are searched by default, with other scholarly-source adapters available. Records are deduplicated, filtered, and ranked locally without an LLM making the paper-selection decision.
* **Bounded review:** A run keeps up to 10 records and creates up to 10 paper cards. It can broaden the search once when too few usable cards are found; a summarization failure alone does not trigger more searching.
* **Lower repeat cost:** Successful paper summaries are cached in PostgreSQL and reused when the source text, question, and prompt version match.
* **Provider resilience:** Groq calls use concurrency and token limits. If configured, OpenRouter gets one fallback attempt when Groq is rate-limited. Runs can still report available cards when some summaries fail.
* **Traceable workflow:** Structured events record workflow steps, source selection, cache use, quote checks, latency, and available model usage in PostgreSQL and the UI.

**Tech stack:** Python, FastAPI, Pydantic, LangGraph, LangChain, Groq, PostgreSQL, React, TypeScript, Vite, Docker Compose.

🔗 **[View Repository](https://github.com/samavinasir/tracereview)**

---

### 🤖 B-vac.AI | Agentic AI for Vaccine Development

> An LLM-orchestrated workflow that chains specialized bioinformatics tools to take a pathogen from genome to prioritized vaccine candidates.

**Problem:** Reverse vaccinology means running many separate tools by hand (genome analysis, protein candidate selection, antigen and epitope evaluation) and combining the results manually.

**What I built:** An agentic workflow that plans the analysis stages, calls the right tools through a unified interface, and produces a ranked list of candidates.

**Engineering highlights**

* LLM-based planning that breaks a pathogen-level goal into tool calls.
* Integration of specialized bioinformatics and machine learning tools into one workflow.
* Retrieval and use of domain-specific scientific resources.
* Multi-stage candidate analysis and prioritization.

<!-- TODO: add one concrete result, e.g. number of pathogens tested or time saved -->

**Tech stack:** Python, LLMs, agentic workflows, machine learning, REST APIs, BLAST, scientific data integration.

---

### 🧠 VacSol-ML | Machine Learning for Vaccine Antigen Prediction

> A machine learning application that predicts vaccine antigen candidates against ESKAPE pathogens. **Published in *Vaccine* (2024).**

**What I built:** The full pipeline: protein feature engineering, model training and validation, integration of specialized prediction tools, a Django web application, and deployment on Linux infrastructure.

**Engineering highlights**

* Protein sequence feature engineering and ML-based candidate prediction.
* Django web application with API and backend integration for computational workflows.
* Packaged as a reusable library on PyPI.
* Deployed and maintained on Linux (Apache + Gunicorn).

<!-- TODO: add the key metric from the paper (e.g. accuracy or AUC and dataset size) -->

**Tech stack:** Python, scikit-learn, Django, PostgreSQL, REST APIs, Linux, Apache, Gunicorn.

📦 **[PyPI Package](https://pypi.org/project/vacsol-ml/)** · 📄 **[Research Publication](https://doi.org/10.1016/j.vaccine.2024.126204)**

---

### 🧬 ProteoAnnot | Protein Annotation Package

> A Python package that wraps sequence-analysis and feature-extraction tools behind one reusable annotation interface, used inside larger AI-assisted research workflows.

**Engineering highlights**

* Integration of Biopython, iFeature and SignalP 6.
* Structured protein feature extraction and annotation output.
* Reusable package and service-oriented design.

**Tech stack:** Python, Biopython, iFeature, SignalP 6, REST APIs.

📦 **[View on PyPI](https://pypi.org/project/proteoannot/)**

<details>
<summary><b>Earlier work</b></summary>

<br>

* **B-Pan:** A Windows desktop application for bacterial pangenome analysis, built with Tkinter and packaged with PyInstaller and Inno Setup. It wraps BLAST, DIAMOND, MUSCLE and MAFFT behind a graphical interface.

</details>

---

## 🛠️ Technical Skills

### AI Engineering & LLM Applications

* Agentic AI and multi-agent workflows
* LangGraph and LangChain
* LLM integration and inference
* Tool calling and workflow orchestration
* Retrieval-augmented generation (RAG)
* Prompt design and structured outputs
* Model evaluation and output validation
* Quantization and QLoRA-based optimization workflows

### Machine Learning & Data Science

* Supervised and unsupervised learning
* Feature engineering and selection
* Model training, evaluation, and validation
* Scikit-learn, XGBoost, LightGBM
* PyTorch and TensorFlow
* Pandas, NumPy, SciPy
* Explainable AI and statistical analysis
* Transformers and representation learning

### Backend & API Engineering

* Python
* FastAPI, Django, Flask
* RESTful API development
* Pydantic and data validation
* Asynchronous processing
* API integration and service design
* Authentication and application architecture

### Data Engineering & Databases

* PostgreSQL, MySQL, SQLite
* pgvector and vector search
* Data processing and transformation
* ETL-style workflows
* Structured data modelling
* Data validation and persistence
* Apache Spark *(currently expanding expertise)*

### Frontend Development

* React
* TypeScript and JavaScript
* HTML5 and CSS3
* Vite
* Bootstrap and Tailwind CSS

### DevOps, Deployment & MLOps

* Docker and Docker Compose
* Linux and Ubuntu server administration
* Git and GitHub
* CI/CD workflows
* Apache2 and Gunicorn
* WSGI application deployment
* On-premises server deployment
* Model versioning and monitoring
* GPU-optimized application deployment

### Scientific AI & Domain Applications

* Scientific literature analysis
* Protein sequence analysis and annotation
* Genomic data processing
* Machine learning for biological datasets
* Scientific workflow automation
* Computational vaccine research

---

## 🧰 Technologies I Work With

<div align="center">

### Languages

<img src="https://skillicons.dev/icons?i=python,typescript,javascript,bash,r"/>

### AI, ML & Data

<img src="https://skillicons.dev/icons?i=pytorch,tensorflow,postgres,mysql,sqlite"/>

### Backend & Frontend

<img src="https://skillicons.dev/icons?i=fastapi,django,flask,react,vite,tailwind"/>

### Infrastructure & Development

<img src="https://skillicons.dev/icons?i=docker,linux,git,github,vscode"/>

</div>

---

## 🏗️ How I Approach AI Engineering

My approach goes beyond connecting an LLM to an API. I focus on the engineering decisions that make an AI application useful in practice.

* **Problem decomposition:** Break complex requirements into manageable components and well-defined workflows.
* **System design:** Select suitable models, tools, databases, and application architecture for the problem.
* **Orchestration:** Coordinate specialized agents and external tools through controlled workflows.
* **Data integrity:** Validate inputs, structure outputs, and persist relevant records.
* **Evaluation:** Identify failure cases and assess the reliability of model outputs and workflow behaviour.
* **Deployment:** Package and deploy applications with attention to reproducibility, resource constraints, and maintainability.
* **Transparency:** Preserve useful source references, execution records, and limitations where appropriate.

I am particularly interested in building AI systems that are not only capable of generating outputs, but can also be evaluated, inspected, and improved.

---

## 📄 Research & Publications

My research background informs how I approach machine learning, scientific data, and AI-assisted applications.

* **VacSol-ML (ESKAPE):** Machine learning for vaccine antigen prediction against ESKAPE pathogens.
  [Read the publication](https://doi.org/10.1016/j.vaccine.2024.126204)

* **Agentic AI and scientific research automation:** Developing workflows that coordinate AI agents and specialized tools to support complex research tasks.

For me, scientific computing is one application area for AI engineering, alongside broader applications in intelligent software, automation, and data-driven systems.

---

## 📊 GitHub Statistics

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=samavinasir&show_icons=true&theme=tokyonight&hide_border=true"/>

<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=samavinasir&layout=compact&theme=tokyonight&hide_border=true"/>

</div>

---

## 🔥 Contribution Streak

<div align="center">

<img src="https://streak-stats.demolab.com?user=samavinasir&theme=tokyonight&hide_border=true"/>

</div>

---

## 🌍 Let's Connect

I'm interested in connecting with teams working on AI engineering, agentic systems, LLM applications, data engineering, and intelligent software products.

<div align="center">

<a href="https://samavinasir.vercel.app/ai"><img src="https://img.shields.io/badge/Portfolio-2563EB?style=for-the-badge&logo=vercel&logoColor=white"/></a>
<a href="https://github.com/samavinasir"><img src="https://img.shields.io/badge/GitHub-475569?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://linkedin.com/in/samavinasir"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:samavi.nasir96@gmail.com"><img src="https://img.shields.io/badge/Email-0EA5A4?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://scholar.google.com/citations?user=K_okdSMAAAAJ&hl=en"><img src="https://img.shields.io/badge/Google%20Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white"/></a>

</div>

---

<div align="center">

### Building AI systems that turn complex problems into practical solutions.

*AI Engineering · Agentic Systems · LLM Applications · Data Engineering*

</div>
