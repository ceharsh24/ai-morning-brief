# AI Morning Brief

This project is a Claude Code-powered AI research agent that generates daily briefs on the latest developments in the AI ecosystem.

## What This Project Does

- Tracks major AI platforms (Claude, Copilot, Codex, Gemini, Cursor, and more)
- Scans AI news, trending GitHub repos, new libraries, agent/MCP frameworks, and research papers
- Generates a formatted markdown report saved to `./ai-briefs/`
- Run `/ai-morning-brief` to trigger a full research scan

## Project Structure

```
ai-morning-brief/
├── CLAUDE.md                          # This file — project context
├── .claude/
│   └── skills/
│       └── ai-morning-brief/
│           └── SKILL.md               # The research agent skill
├── ai-briefs/                         # Generated reports land here
│   └── .gitkeep
└── README.md
```

## Key Commands

- `/ai-morning-brief` — Run the full research scan and generate today's report
- `/ai-morning-brief focus on multi-agent orchestration` — Run with a specific focus area

## Notes

- Reports are saved as `ai-briefs/brief-YYYY-MM-DD.md`
- The skill uses WebFetch to pull from Hacker News, GitHub Trending, HuggingFace Papers, arXiv, and more
- Each report ends with key takeaways and top links worth reading
