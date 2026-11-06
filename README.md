<h1 align="center">Ali Merhej</h1>
<p align="center"><b>Backend & AI Systems Engineer</b></p>
<p align="center">Building reliable AI systems: from data and architecture to agents and the interfaces people actually use.</p>

<p align="center">
  <a href="https://www.linkedin.com/in/ali-merhej-8615943b7"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:mrhj26ali@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## About

I'm a final-year B.Eng. student in AI and Software Engineering at HIAST (Damascus, Syria), working remotely. I'm interested in the part of AI that comes after the demo: building AI systems and the infrastructure behind them so they are **trustworthy, observable, and safe to run in production**.

My work sits where backend architecture meets applied AI. I like clean boundaries between components, systems that fail gracefully, and AI that is validated and accountable rather than merely impressive.

**Where I'm heading:** AI infrastructure, MLOps, and AI security, ideally through a Master's program.

I'm always open to learning new languages, frameworks, and tools as a problem requires them.

---

## Featured Work

### BuildPolaris: AI-enabled construction management platform
*Founder & Lead Engineer · 2025 – present*

An enterprise platform I architected end to end as three independent codebases with explicit contracts between them:

| Layer | What it does | Stack |
| :-- | :-- | :-- |
| **Backend (system of record)** | Layered modular monolith covering scheduling (critical-path method), financials, document control, field operations and closeout. Exposes an MCP server so the AI layer can call backend operations as tools, and every write is re-validated against live permissions. | Frappe, ERPNext v16, MariaDB |
| **AI service** | Stateless sidecar on hexagonal architecture that holds no authoritative data. Hybrid retrieval (vector + graph + rank fusion) and a LangGraph agent system with human-in-the-loop approval gates, citation validation before answers are returned, and automatic failover across five LLM providers. | Python, FastAPI, pgvector, Apache AGE, LangGraph |
| **Offline-first frontend** | Field-execution screens that behave identically online and offline. The scheduling algorithm also runs client-side in a Web Worker for instant Gantt feedback, kept consistent with the backend through a shared golden test suite. | React 19, TypeScript, RxDB, Vite |

**Engineering decision worth sharing:** pure vector search failed on multi-hop questions such as "which delayed tasks have open safety incidents?". Adding graph traversal and Reciprocal Rank Fusion to the retrieval pipeline resolved it.

### Mizan: an Arabic-native language for industrial control
A compiled, statically typed domain-specific language for industrial process monitoring. The full pipeline runs from an ANTLR4 grammar through the AST, semantic analysis (physical-unit type checking, finite-state-machine enforcement) and LLVM IR to native code, linked against libmodbus and libmosquitto. It includes a GUI Modbus TCP plant simulator for hardware-free testing.

### Other projects
- **LMS Backend:** ASP.NET Core Web API using Clean Architecture, CQRS (MediatR), JWT with role-based access control, dual SQL Server databases, and English/Arabic localization.
- **Student Information System:** .NET 10 and Entity Framework Core with a layered Clean Architecture design.

---

## Research Experience

**Research Assistant, Damascus University (2025)**, Faculty of Engineering.
Supported PhD-level research alongside master's candidates on predictive modeling and planning under uncertainty, including a fuzzy neural network approach to prediction that was later extended toward LLM-based and simulation methods. Contributed across the pipeline, from model design and implementation to evaluation.

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**AI & Data**

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL%20%2F%20pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)

**Backend & Frontend**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Frappe](https://img.shields.io/badge/Frappe%20%2F%20ERPNext-0089FF?style=flat-square&logo=erpnext&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)

**Infrastructure & Tooling**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![LLVM](https://img.shields.io/badge/LLVM-262D3A?style=flat-square&logo=llvm&logoColor=white)

**Practices:** Clean and hexagonal architecture · CQRS · RAG and hybrid retrieval · agentic systems with human-in-the-loop safety · offline-first design · JWT and RBAC

---

## Currently

- Deepening my skills in AI infrastructure, MLOps and AI security
- Looking for Master's program opportunities in these areas
- Open to collaboration, research, and remote engineering roles




