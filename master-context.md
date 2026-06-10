# Master Context — AI Learning Journey

## Who I am
- Complete beginner — no coding background
- Rarely use terminal
- Using a company-owned Mac (company-owned)
- Learning on personal time to future-proof career

## My Goals
- Get a new job in AI/agentic AI space
- Build automation skills companies are asking for
- 30-60 mins/day available for learning
- Target profile: "The Orchestrator" — no-code/low-code 
  AI workflow builder. Realistic in 3-6 months.

## My Setup
- Mac (company-owned)
- Docker Desktop installed
- Ollama running locally (llama3)
- n8n self-hosted via Docker
  - Start with: docker start -ai n8n
  - Access at: http://localhost:5678
- Claude Code installed

## My Two Claude Accounts
- Personal: claude-p
- Work: claude-w
- Rule: NEVER use claude-w for personal learning
- Aliases set up in ~/.zshrc

## Folder Structure
~/Desktop/claude/
├── personal/   ← all personal learning projects
└── work/       ← company work only

## GitHub
- Repo: https://github.com/<link>
- Committing directly via github.com (no cloning on work laptop)
- Daily progress logged in progress-log.md
- This master context lives in master-context.md
- Daily progress logged as YYYYMMDD-progress.md (e.g. 20260526-progress.md)

## Learning Plan

### Phase 1 — Foundation (Weeks 1-4)
Goal: Understand how AI workflows work
- Build 3-4 small n8n workflows
- Get comfortable with nodes, triggers, expressions
- Output: 4 working workflows documented on GitHub

### Phase 2 — Going Deeper (Weeks 5-8)
Goal: Build something genuinely useful
- Connect n8n to real tools (Slack, Gmail, Notion)
- Build one workflow used daily
- Learn AI agent concepts: memory, tools, loops
- Output: 1 real tool I actually use

### Phase 3 — Portfolio (Weeks 9-12)
Goal: Have something to show in interviews
- Polish one project end to end
- Document clearly on GitHub
- Be able to explain it in an interview
- Output: 2-3 portfolio projects with documentation

## How Claude Code Fits In
Not a separate track — it's my assistant while building.
n8n for workflow structure → Claude Code for custom logic

## My Preferences (for AI assistant)
- Treat me as a complete beginner
- One step at a time, no overwhelming concepts
- Practical and project-based always
- High level overview first, then details
- Remind me to commit to GitHub after every session
- Keep costs low, prefer local/self-hosted
- Suggest opening a new thread if conversation gets too long
- Start each new thread with current progress

## What I've Built
1. Manual Trigger → Edit Fields → Basic LLM Chain (v1 summarizer)
2. Chat Trigger → Basic LLM Chain (v2 summarizer)
3. Thai Slack Summarizer — translates Thai → English bullets
4. Memory Chat Assistant — AI Agent + Simple Memory

## Current Status
Phase 1 complete
Starting Phase 2 next session

## n8n on Oracle Cloud VM
- Access: `http://<duckdns-domain>:<port>`
- SSH: `ssh -i <path-to-private-key> ubuntu@<oracle-vm-ip>`
- Restart command:
  `docker stop n8n && docker rm n8n`
- Run command:
```
  docker run -d \
    --name n8n \
    --env-file ~/n8n.env \
    -p 5678:5678 \
    -v n8n_data:/home/node/.n8n \
    n8nio/n8n
```
- Env file location: `~/n8n.env`
- Required env vars: `N8N_PROTOCOL, N8N_HOST, N8N_PORT, 
  N8N_SECURE_COOKIE, WEBHOOK_URL, APIFY_API_TOKEN, 
  GEMINI_API_KEY, RESUME_URL, GMAIL_SENDER, GMAIL_RECIPIENT`
