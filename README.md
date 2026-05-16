# Autonomous Job Matcher 

Automated pipeline that scrapes job boards, scores offers against my profile using LLM, and delivers top matches via Discord every morning.

## Architecture

scrapers → PostgreSQL → Groq/Llama3 → Discord Webhook

## Tech Stack

- Python 3.12, FastAPI
- Playwright (scraping)
- SQLAlchemy + PostgreSQL
- Groq API (Llama 3)
- APScheduler, Discord Webhook
- Docker

## Setup

1. Clone the repo
2. Copy `.env.example` to `.env` and fill in the values
3. `docker-compose up -d`
4. `pip install -r requirements.txt`
5. `python -m app.main`

## Status

In active development