# CryptoTradeLogger

![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Redis 6.0+](https://img.shields.io/badge/Redis-6.0%2B-red?logo=redis&logoColor=white)

A lightweight, real‑time cryptocurrency trade logger backed by Redis for ultra‑low‑latency storage and retrieval.

---


## Key Features
- **Real‑time capture** of trades from supported exchanges.  
- **Redis storage** for millisecond‑level writes/reads.  
- **Configurable retention** (keep the latest *N* trades).  
- **Minimal dependencies** and single‑file entry point.  
- **Easily extensible** for additional markets or data pipelines.  

---

## Requirements
| Software | Version | Notes |
| -------- | ------- | ----- |
| Python   | 3.8 or newer | Install from [python.org](https://www.python.org/) or via `pyenv`/system package manager. |
| Redis    | 6.0 or newer | Local service, Docker container, or managed instance. |

> **Tip:** On Linux/macOS you can spin up Redis instantly with  
> `docker run -p 6379:6379 redis`.

---

## Quick Start
```bash
# 1 — Clone the repository
git clone https://github.com/Satviksangamkar/CryptoTradeLogger.git
cd CryptoTradeLogger

# 2 — Install Python dependencies
pip install -r requirements.txt

# 3 — Run the logger (uses localhost:6379 by default)
python task.py


