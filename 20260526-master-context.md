# My AI Learning Journey - Master Context

## Who I am
- Complete beginner — no coding background
- Rarely use terminal
- Work at LINE MAN Wongnai (Bangkok)
- Using a company-owned Mac
- Learning on personal time to future-proof career

## My Goal
- Get a new job in AI/agentic AI space
- Build automation skills companies are asking for
- 30-60 mins/day available for learning

## My Setup
- Mac (company-owned)
- Docker Desktop installed
- Ollama running locally (llama3)
- n8n self-hosted via Docker
  - Start with: docker start -ai n8n
- Claude Code installed

## My Two Claude Accounts
- Personal: claude-p (gauravbansal1410@gmail.com, Pro)
- Work: claude-w (gaurav.b@lmwn.com, Team)
- Rule: NEVER use claude-w for personal learning
- Aliases set up in ~/.zshrc

## Folder Structure
~/Desktop/claude/
├── personal/   ← all personal learning projects
└── work/       ← company work only

## GitHub
- Repo: https://github.com/gauravbansal1410/learning-ai-agents
- Committing daily learning logs as .md files
- Committing directly via github.com (not cloning on work laptop)

## What I've Already Built
1. n8n: Manual Trigger → Basic LLM Chain → Ollama Chat Model
   (local AI workflow, working)
2. Claude Code: Text Summarizer
   - Folder: ~/Desktop/claude/personal/summarizer/
   - Uses Ollama + llama3 (free, local)
   - Outputs bullet point summary to output.txt

## What I Already Know
- Docker runs containers, n8n runs inside Docker
- Ollama runs separately from Docker
- Execute Step vs Execute Workflow in n8n
- mkdir -p, source ~/.zshrc, basic terminal commands
- Basic Markdown (headings, lists, code blocks, checklists)
- What Claude Code is: AI that acts, not just answers

## Learning Plan

### Target Profile
"The Orchestrator" — builds AI workflows using no-code/low-code
tools. Realistic in 3-6 months. Genuinely in demand.

### Phase 1 — Foundation (Weeks 1-4)
Goal: Understand how AI workflows work
- Finish n8n summarizer project
- Build 3-4 small n8n workflows
- Get comfortable with nodes, triggers, agents
- Output: 4 working workflows on GitHub

### Phase 2 — Going Deeper (Weeks 5-8)
Goal: Build something genuinely useful
- Connect n8n to real tools (Gmail, Notion, Google Sheets)
- Build one workflow used daily
- Learn AI agent concepts: memory, tools, loops
- Use Claude Code to help customize
- Output: 1 real tool I actually use

### Phase 3 — Portfolio (Weeks 9-12)
Goal: Have something to show in interviews
- Polish one project
- Document properly on GitHub
- Be able to explain it clearly
- Explore Make.com or simple Python agent
- Output: 2-3 portfolio projects with documentation

## How Claude Code Fits In
Not a separate track — it's my assistant while building.
n8n for workflow structure → Claude Code for custom logic

## Current Status
- Phase 1, Week 1
- Next task: Finish n8n summarizer (Manual Trigger → 
  Text Input → AI Summarizer → Output)

## My Preferences (for AI assistant)
- Treat me as a complete beginner
- One step at a time
- No overwhelming concepts
- Practical and project-based
- High level overview first, then details
- Remind me to commit to GitHub after sessions
- Keep costs low, prefer local/self-hosted
