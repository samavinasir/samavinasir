<div align="center">

# Samavi Nasir

### AI Engineer · Agentic AI · LLM Applications · Data Engineering

I build AI-powered applications, agentic workflows, and data-driven systems, from model development and orchestration to APIs, databases, and deployment.

<br />

<a href="https://samavinasir.vercel.app/ai"><img src="https://img.shields.io/badge/Portfolio-2563EB?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" /></a>
<a href="https://linkedin.com/in/samavinasir"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://scholar.google.com/citations?user=K_okdSMAAAAJ&hl=en"><img src="https://img.shields.io/badge/Google%20Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Google Scholar" /></a>
<a href="mailto:samavi.nasir96@gmail.com"><img src="https://img.shields.io/badge/Email-0EA5A4?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

</div>

<br />

<img src="assets/banners/01-about-me.svg" alt="01 / About" width="100%" />

I'm an **AI Engineer** who turns complex requirements into working, inspectable software. My work spans the full AI lifecycle: data processing and model development, agent orchestration, backend engineering, database design, and deployment on Linux infrastructure.

My background is in applied machine learning and scientific computing, where I built and published AI tools for computational vaccine design. I now apply that rigor to broader AI engineering: agentic systems, LLM-powered tools, and research automation.

**Currently focused on**

- 🤖 Agentic AI and multi-agent orchestration with LangGraph and LangChain
- 🧠 LLM applications, RAG, and tool-using agents
- ⚙️ Backend engineering and AI-powered APIs
- 🗄️ Data engineering with PostgreSQL and vector databases
- 🐳 Docker, CI/CD, and production-oriented deployment
- 📊 Model evaluation and MLOps

<br />

<img src="assets/banners/02-featured-projects.svg" alt="02 / Projects" width="100%" />

### TraceReview · *Literature review you can trace*

Ask a research question and get a focused set of papers as source-checked reading cards, with every workflow step inspectable. Built as a controlled LangGraph workflow that searches PubMed and Europe PMC, then selects up to 10 papers and turns them into cards with an AI study summary and source-matched excerpts.

- **Checked excerpts:** proposed quotes are verified against the abstract, with verbatim fallback when they don't match.
- **Focused retrieval:** records are deduplicated, filtered, and ranked locally, so no LLM decides which papers are selected.
- **Inspectable runs:** structured events for steps, cache use, quote checks, and latency are stored in PostgreSQL and shown in the UI.

`Python` `FastAPI` `LangGraph` `LangChain` `Groq` `PostgreSQL` `React` `TypeScript` `Docker Compose`

🔗 **[View repository](https://github.com/samavinasir/tracereview)**

<br />

### B-vac.AI · *Agentic AI for vaccine development*

An LLM-orchestrated workflow that chains specialized bioinformatics tools to take a pathogen from genome to prioritized vaccine candidates. Reverse vaccinology normally means running many separate tools by hand; this plans the analysis stages, calls the right tools through one interface, and returns a ranked candidate list.

- LLM-based planning that breaks a pathogen-level goal into tool calls.
- Integration of bioinformatics and machine learning tools into a single workflow.
- Multi-stage candidate analysis and prioritization using domain-specific scientific resources.

<!-- Add one concrete result here, e.g. number of pathogens tested or time saved, plus a repo link if public. -->

`Python` `LLMs` `Agentic workflows` `Machine learning` `REST APIs` `BLAST`

<br />

### B-vac · *Reverse vaccinology, simplified*

A standalone, offline desktop application for bacterial vaccine candidate discovery. It screens proteomes through subcellular localization, non-host homology, virulence factor analysis, and epitope mapping, with no command line or internet connection required. Ships as executables for Windows and Linux. **Published in *Scientific Reports* (2025).**

`Python` `Tkinter` `PyInstaller`

🔗 **[Repository](https://github.com/samavinasir/b-vac)** &nbsp;·&nbsp; 💻 **[Download](https://samavinasir.github.io/b-vac)** &nbsp;·&nbsp; 📄 **[Paper](https://doi.org/10.1038/s41598-025-01201-0)**

<br />

### VacSol-ML · *Machine learning for vaccine antigen prediction*

Predicts vaccine antigen candidates against ESKAPE pathogens. I built the full pipeline: protein feature engineering, model training and validation, integration of prediction tools, a Django web application, and Linux deployment (Apache + Gunicorn). Packaged as a reusable library on PyPI. **Published in *Vaccine* (2024).**

<!-- Add the key metric from the paper here (e.g. accuracy or AUC and dataset size). -->

`Python` `scikit-learn` `Django` `PostgreSQL` `Linux` `Gunicorn`

📦 **[PyPI](https://pypi.org/project/vacsol-ml/)** &nbsp;·&nbsp; 📄 **[Publication](https://doi.org/10.1016/j.vaccine.2024.126204)**

<br />

### ProteoAnnot · *Protein annotation package*

A Python package that wraps Biopython, iFeature, and SignalP 6 behind one reusable annotation interface, with structured feature-extraction output. Used inside larger AI-assisted research workflows.

`Python` `Biopython` `iFeature` `SignalP 6` `REST APIs`

📦 **[PyPI](https://pypi.org/project/proteoannot/)**

<details>
<summary><b>Earlier work</b></summary>

<br />

- **B-Pan:** a Windows desktop application for bacterial pangenome analysis, built with Tkinter and packaged with PyInstaller and Inno Setup. It wraps BLAST, DIAMOND, MUSCLE, and MAFFT behind a graphical interface.

</details>

<br />

<img src="assets/banners/03-technical-skills.svg" alt="03 / Skills" width="100%" />

| Area | Tools and practices |
|:--|:--|
| **AI & LLMs** | Agentic workflows · LangGraph · LangChain · RAG · tool calling · structured outputs · output validation |
| **ML & Data Science** | scikit-learn · XGBoost · LightGBM · PyTorch · TensorFlow · Pandas · NumPy · SciPy |
| **Backend & APIs** | Python · FastAPI · Django · Flask · REST design · Pydantic · async processing |
| **Data & Databases** | PostgreSQL · pgvector · MySQL · SQLite · ETL workflows · Apache Spark *(learning)* |
| **Frontend** | React · TypeScript · JavaScript · Vite · Tailwind CSS |
| **DevOps & MLOps** | Docker · Docker Compose · Linux/Ubuntu servers · Git · CI/CD · Apache2 · Gunicorn |
| **Scientific domains** | Protein sequence analysis · genomic data processing · scientific literature analysis · computational vaccine research |

<div align="center">

<img src="https://skillicons.dev/icons?i=python,typescript,javascript,r,bash,pytorch,tensorflow,postgres,fastapi,django,flask,react,vite,tailwind,docker,linux,git,github&perline=9" alt="Technology icons" />

</div>

<br />

<img src="assets/banners/04-how-i-build.svg" alt="04 / Approach" width="100%" />

My approach goes beyond connecting an LLM to an API. I focus on the decisions that make an AI application useful in practice:

- **Design first:** break complex requirements into well-defined workflows, then choose models, tools, and databases to fit.
- **Controlled orchestration:** coordinate agents and external tools through bounded, predictable workflows instead of open-ended loops.
- **Validate everything:** check inputs, structure outputs, persist records, and test failure cases.
- **Stay inspectable:** keep source references, execution records, and stated limitations so results can be evaluated and improved.

<br />

<img src="assets/banners/05-publications.svg" alt="05 / Research" width="100%" />

- **B-vac: A robust software package for bacterial vaccine design.** Ali, A., Hamid, M. H. B., Nasir, S., Ishaq, Z., & Anwer, F. (2025). *Scientific Reports*, 15, 31745. [10.1038/s41598-025-01201-0](https://doi.org/10.1038/s41598-025-01201-0)
- **VacSol-ML (ESKAPE pathogens):** machine learning for vaccine antigen prediction. *Vaccine* (2024). [10.1016/j.vaccine.2024.126204](https://doi.org/10.1016/j.vaccine.2024.126204)

Full list on [Google Scholar](https://scholar.google.com/citations?user=K_okdSMAAAAJ&hl=en).

<br />

<img src="assets/banners/06-let-s-connect.svg" alt="06 / Contact" width="100%" />

I'm interested in connecting with teams working on AI engineering, agentic systems, LLM applications, data engineering, and intelligent software products.

📬 [Email](mailto:samavi.nasir96@gmail.com) &nbsp;·&nbsp; 💼 [LinkedIn](https://linkedin.com/in/samavinasir) &nbsp;·&nbsp; 🌐 [Portfolio](https://samavinasir.vercel.app/ai) &nbsp;·&nbsp; 🎓 [Google Scholar](https://scholar.google.com/citations?user=K_okdSMAAAAJ&hl=en)

<br />

---

<div align="center">

**Building AI systems that turn complex problems into practical solutions.**

<sub>AI Engineering · Agentic Systems · LLM Applications · Data Engineering</sub>

</div>
