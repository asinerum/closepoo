# ClosePoo: Simple-as-poo AI Agent

We don't use OpenClaw, because we have ClosePoo, a simple-as-poo AI Agent that makes your time easy and controllable.

## Prerequisites

Python 3.10 with Pip 25.0.0 fresh installed and added to PATH

## Clone Poo Repo with Simplest Samples

```bash
git clone https://github.com/asinerum/closepoo
cd closepoo
```

## Install Poo

```bash
pip install closepoo
```

## Edit Poo Configuration

```bash
nano .env
```

The main Poo configs be seen as follows:

```ts
## .env
GEMINI_API_KEY = "YOUR_GEMINI_API_KEY_HERE"
TELEGRAM_BOT_TOKEN = "YOUR_TELEGRAM_BOT_TOKEN_HERE"
TELEGRAM_AUTH_USER_LIST = [YOUR_TELEGRAM_ID_LIST_HERE]
```

## Import AI Skills

Any public Claude-style AI skill is acceptable

```ts
## Python
from closepoo import setup_skills
setup_skills("https://github.com/googleworkspace/cli.git")
```

## Select AI Skills

Copy only needed skills into subfolder named ./skills_cache/skills/

## Start Web Chatbot

```bash
streamlit run webchat.py
```

## Start Telegram Chatbot

```bash
python telechat.py
```

(C)2026 ASINERUM CONLANG PROJECT
