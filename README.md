## 👋 Hi, I'm Youssef Tadros

I'm a **Python developer** with a strong focus on backend systems and automation. I love writing clean, testable code that solves complex problems, especially in data engineering and infrastructure-heavy environments. My professional background includes building scalable data pipelines on AWS and automating tricky data ingestion workflows. I'm currently looking for developer roles where I can keep growing and shipping useful systems.

```python
def solve(problem):
    constraints = extract_constraints(problem)
    try:
        logic = apply_deduction(constraints)
        return solution
    except CustomError:
        tie_loose_ends()
        raise CustomError

# this is my idea of fun
```

---

### 🔧 Recent Professional Work

From June 2022 to March 2025, I was a Python Developer on a federal contract with NOAA through Cloud Alliance Inc.

I built and maintained AWS-based data pipelines that processed data from a wide variety of providers. These included:

- **Scanner pipelines**, which handled format validation, hash and integrity checks, and virus scanning before data moved to our “clean” S3 bucket. These pipelines were designed to be provider-agnostic, scalable via deployment in an EKS cluster, and monitored using CloudWatch alarms on associated SQS queues.
- **Pulling pipelines**, which retrieved data from external sources that couldn't push to our "dirty" bucket. These pipelines were more complex and provider-specific. I developed several of them myself, fetching data from **https**, **ftps**, and **sftp** sources. These were my favorite tasks—where I got to be creative and dive deep into problem solving.

My final project involved a **Tectia SFTP server** that required command-line access via a proprietary tool. I developed Python classes using **pexpect** to establish and manage subprocess connections, authenticate, retrieve directory listings, download files, and gracefully close connections—all while keeping the session alive and stable throughout.

I leaned heavily on:
- **Object-oriented design** using abstract base classes and dynamic module loading
- **Unit testing** with unittest and mock objects for SFTP behaviors
- **Log-driven triage** — Used structured logs, egrep, and DLQ analysis to resolve production issues flagged by CloudWatch alarms

---

### 🔍 Notable Engineering Challenges at NOAA

- **S3 Multipart Upload Validator** — Solved silent checksum failures for large S3 uploads by building a custom chunked validator using `boto3`. This restored data integrity across high-throughput ingest pipelines and eliminated DLQ-triggered alarms.

- **Tectia SFTP Automation** — Automated file ingestion from a proprietary CLI-only SFTP server by building a Python client with `pexpect`. Managed authentication and file transfers in ephemeral container environments without API access.


### 🧠 Personal Projects

#### 🔍 [Auto-Minesweeper (Python)](https://github.com/ytadros/Auto-Minesweeper)
A Minesweeper solver that includes options to visualize the logic engine's moves and tweak strategies on the fly. Features include:
- Board and logic engine customization
- Live logic visualization and dynamic step pacing
- Hyper-solve mode for advanced overlapping neighbor set reasoning
- Currently undergoing a refactor to adopt MVC separation, performance profiling (`cProfile`), and CI/test coverage using `unittest` and GitHub Actions

##### 🎥 Visual Demo
**Solver in Action** — Logic unfolds with live step control and visual feedback  
![Solver in Action](https://github.com/ytadros/Auto-Minesweeper/raw/main/minesweeper_gameplay_1.gif)

**Custom + Directional Solve** — Demonstrates first-click safety and rule-based directional solving  
![Custom + Directional Solve](https://github.com/ytadros/Auto-Minesweeper/raw/main/minesweeper_gameplay_2.gif)

#### 🗂️ Orientations Aggregator (Python, Spring 2022)
Developed a spreadsheet-configurable tool to consolidate orientation event data for an adult literacy nonprofit. Designed for non-technical users with one-click execution and six months of post-installation support. (Pending open-source release.)

---

### 🛠️ Technical Skills

**Languages**: Python, SQL, Bash  
**Cloud & Infrastructure**: AWS (S3, EKS, SQS, CloudWatch), Docker, Kubernetes, Linux  
**Tools & Libraries**: unittest, logging, boto3, paramiko, ftplib, requests, pandas, pexpect, subprocess  
**Protocols**: HTTP/S, FTPS, SFTP, Tectia SFTP (CLI)  
**Practices**: CI/CD basics, Agile workflows, testability, clean architecture

---

### 💡 How I Work

I thrive in backend environments where systems are invisible when they work—but critical when they fail. I like pipelines that heal themselves, logs that tell stories, and abstractions that explain themselves. I debug by making systems observable and structure code with future readers in mind.

---

### 📫 How to Reach Me

**Email**: youssef.s.tadros@gmail.com  
**LinkedIn**: [linkedin.com/in/youssef-tadros](https://www.linkedin.com/in/youssef-tadros/)
