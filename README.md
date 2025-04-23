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

### 🔧 Recent Professional Work

From June 2022 to March 2025, I was a Python Developer on a federal contract with NOAA through Cloud Alliance Inc.

I built and maintained AWS-based data pipelines that processed data from a wide variety of providers. These included:

- **Scanner pipelines**, which handled format validation, hash and integrity checks, and virus scanning before data moved to our “clean” S3 bucket. These pipelines were designed to be provider-agnostic, scalable via deployment in an EKS cluster, and monitored using CloudWatch alarms on associated SQS queues.

- **Pulling pipelines**, which retrieved data from external sources that couldn't push to our "dirty" bucket. These pipelines were more complex and provider-specific. I developed several of them myself, fetching data from **https**, **ftps**, and **sftp** sources. These were my favorite tasks—where I got to be creative and dive deep into problem solving.

My final project involved a **Tectia SFTP server** that required command-line access via a proprietary tool. I developed Python classes using **pexpect** to establish and manage subprocess connections, authenticate, retrieve directory listings, download files, and gracefully close connections—all while keeping the session alive and stable throughout.

I leaned heavily on:

- **Unit testing**, including mocking tricky behaviors and simulating infrastructure.
- **Python’s logging module**, to output clean, structured logs that made debugging and monitoring straightforward.

### 🧠 Personal Projects

**🔍 Auto-Minesweeper (Python) (In Development)**  
A Minesweeper player that includes options to visualize the logic engine's moves and tweak it on the fly. Features include:
- Board customization options
- Logic engine customization and visual debugging options
- Currently expanding with unit tests, performance optimizations, and–crucially–a more modular code structure

### 🛠️ Technical Skills

**Languages**: Python, SQL, Bash  
**Cloud & Infrastructure**: AWS (S3, EKS, SQS, CloudWatch), Docker, Kubernetes, Linux
**Tools & Libraries**: unittest, logging, boto3, paramiko, ftplib, requests, pandas, pexpect, subprocess, multiprocessing
**Protocols**: HTTP/S, FTPS, SFTP, Tectia SFTP (CLI)  
**Other**: Git, VS Code, Agile, Data Pipelines, CI/CD basics
