# 🛰️ AI Morning Brief

A Claude Code project that acts as your personal AI research agent. Run one slash command and get a comprehensive daily digest of what's happening in AI.

## Quick Start

```bash
# Clone the project
git clone https://github.com/YOUR_USERNAME/ai-morning-brief.git
cd ai-morning-brief

# Open Claude Code
claude

# Run the research agent
/ai-morning-brief
```

## What It Researches

|Category           |Sources                                                     |
|-------------------|------------------------------------------------------------|
|📡 AI News          |Hacker News, The Verge, TechCrunch, Reddit r/MachineLearning|
|🔥 GitHub Repos     |GitHub Trending (Python, TypeScript, weekly)                |
|📦 Libraries & Tools|LangChain, LlamaIndex, AutoGen, CrewAI, HuggingFace, etc.   |
|🤖 Agents & MCP     |MCP servers, A2A protocol, multi-agent frameworks           |
|🧪 Research Papers  |HuggingFace Papers, arXiv (cs.AI, cs.CL)                    |

## Output

Each run produces:

- **Terminal summary** — top 3-5 items per category printed to your screen
- **Markdown report** — detailed brief saved to `ai-briefs/brief-YYYY-MM-DD.md`

## Automate (Optional)

Run it every morning without opening Claude Code:

```bash
# Add to crontab -e
0 7 * * * cd ~/ai-morning-brief && claude -p "/ai-morning-brief" --dangerously-skip-permissions 2>&1 >> ai-briefs/cron.log
```

## Customize

Edit `.claude/skills/ai-morning-brief/SKILL.md` to:

- Add/remove research sources
- Change focus areas (e.g., emphasize multi-agent orchestration)
- Modify the report template
- Add email delivery via bash

## Project Structure

```
ai-morning-brief/
├── CLAUDE.md                              # Project context for Claude Code
├── README.md                              # This file
├── .claude/
│   ├── settings.json                      # Permission pre-approvals
│   └── skills/
│       └── ai-morning-brief/
│           └── SKILL.md                   # The research agent skill
└── ai-briefs/                             # Generated reports
    └── .gitkeep
```

## License

MIT
