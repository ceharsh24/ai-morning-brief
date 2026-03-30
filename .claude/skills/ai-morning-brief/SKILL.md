---
name: ai-morning-brief
description: Research the latest AI developments — platform updates (Claude, Copilot, Codex, Gemini), discover new skills/agents/MCP servers, scan trending GitHub repos, new libraries, and research papers — then generate a formatted daily brief report.
allowed-tools: WebFetch, Bash, Read, Write, Glob
---

# AI Morning Brief — Research Agent

You are an AI research agent. Your job is to scan the AI ecosystem and produce a comprehensive daily brief.

## Research Categories

Research ALL of the following categories. For each, use WebFetch to gather the latest information:

### 1. 📡 AI News & Announcements

Search for: latest AI news today, major model releases, company announcements, funding rounds, policy updates, partnerships.
Sources to check:

- https://news.ycombinator.com (Hacker News front page)
- https://www.theverge.com/ai-artificial-intelligence
- https://techcrunch.com/category/artificial-intelligence/
- https://www.reddit.com/r/MachineLearning/hot/
- https://www.reddit.com/r/artificial/hot/
- https://www.reddit.com/r/LocalLLaMA/hot/
- https://www.reddit.com/r/singularity/hot/
- https://9to5google.com/guides/ai/ (Google AI news)
- https://www.tomsguide.com/ai (mainstream AI coverage)

### 2. 🏢 AI Platforms & Developer Tools Tracker

This is a HIGH PRIORITY category. Track the latest from every major AI platform and coding tool:

#### Anthropic / Claude

- Claude model updates (Opus, Sonnet, Haiku — new versions, capabilities, benchmarks)
- Claude Code updates (new skills, slash commands, hooks, plugins, subagents, MCP integrations)
- Claude API changes (new features, pricing changes, rate limits, SDK updates)
- Claude.ai product updates (Projects, Artifacts, computer use, new features)
- Anthropic research, blog posts, and policy announcements
- Sources: https://www.anthropic.com/news, https://docs.anthropic.com/en/docs/about-claude/models, https://www.npmjs.com/package/@anthropic-ai/claude-code
- Reddit: https://www.reddit.com/r/ClaudeAI/hot/, https://www.reddit.com/r/anthropic/hot/

#### GitHub Copilot

- Copilot model updates and capability changes
- Copilot Chat, Copilot Workspace, Copilot CLI updates
- New Copilot agents, skills, and extensions
- Copilot for PRs, code review, and documentation features
- Enterprise/Business tier changes and new features
- GitHub Next experiments and previews
- Sources: https://github.blog/tag/github-copilot/, https://github.com/features/copilot
- Reddit: https://www.reddit.com/r/GithubCopilot/hot/, https://www.reddit.com/r/vscode/hot/

#### OpenAI / Codex / ChatGPT

- New model releases (GPT-4.x, o-series reasoning models, new modalities)
- Codex CLI agent updates and capabilities
- ChatGPT product updates (canvas, memory, plugins, custom GPTs)
- OpenAI API changes (new endpoints, function calling updates, pricing)
- OpenAI Agents SDK and Swarm framework updates
- Sources: https://openai.com/blog, https://platform.openai.com/docs/changelog
- Reddit: https://www.reddit.com/r/OpenAI/hot/, https://www.reddit.com/r/ChatGPT/hot/, https://www.reddit.com/r/ChatGPTCoding/hot/

#### Google / Gemini

- Gemini model updates (Pro, Ultra, Flash, Nano)
- Gemini CLI agent and agentic capabilities
- Google AI Studio and Vertex AI updates
- Android AI / on-device AI features
- NotebookLM, AlphaFold, DeepMind research
- Sources: https://blog.google/technology/ai/, https://ai.google.dev/
- Reddit: https://www.reddit.com/r/Bard/hot/, https://www.reddit.com/r/GoogleGeminiAI/hot/

#### Other AI Platforms & Tools

- **Cursor** — IDE updates, model integrations, agent mode changes
- **Windsurf (Codeium)** — editor updates, Cascade agent, new features
- **Aider** — new releases, model support, benchmarks
- **Bolt / Lovable / v0** — AI app builder updates
- **Replit Agent** — deployment and development agent updates
- **Amazon Q Developer / CodeWhisperer** — AWS AI coding tools
- **JetBrains AI / Junie** — IDE AI assistant updates
- **Sourcegraph Cody** — code intelligence updates
- **Tabnine** — AI assistant updates
- **Devin (Cognition)** — autonomous agent developments
- **Mistral / Meta Llama / Cohere / xAI Grok** — open and closed model releases
- Reddit for AI coding tools: https://www.reddit.com/r/cursor/hot/, https://www.reddit.com/r/CodingWithAI/hot/, https://www.reddit.com/r/ArtificialIntelligence/hot/

### 3. 🔥 Trending GitHub Repos

Search for: trending AI/ML GitHub repositories this week.
Sources to check:

- https://github.com/trending?since=weekly
- https://github.com/trending/python?since=weekly
- https://github.com/trending/typescript?since=weekly
  Look for repos related to: LLMs, agents, MCP, A2A, fine-tuning, RAG, evaluation, orchestration, CLI agents, code generation.

### 4. 📦 New Libraries, SDKs & Tools

Search for: new releases and version updates in the AI/LLM ecosystem.
Check release pages and changelogs for:

- LangChain, LlamaIndex, AutoGen, CrewAI, Semantic Kernel, AG2
- Hugging Face transformers, vLLM, Ollama, LM Studio
- Anthropic SDK, OpenAI SDK, Google AI SDK, Vercel AI SDK
- Instructor, Outlines, LMQL, Guidance (structured output tools)
- DSPy, PromptFlow, Haystack (prompt/pipeline frameworks)
- Any new PyPI or npm packages gaining traction in AI space

### 5. 🤖 AI Agents, MCP & A2A

Search for: latest developments in AI agent frameworks, MCP servers, A2A protocol, multi-agent orchestration.
Focus on:

- New MCP server releases and integrations
- A2A (Agent-to-Agent) protocol updates and implementations
- Multi-agent frameworks and orchestration tools (AutoGen, CrewAI, LangGraph, OpenAI Swarm)
- Claude Code skills/plugins ecosystem
- CLI agent landscape (Claude Code, GitHub Copilot CLI, Gemini CLI, Codex CLI, Aider)
- Agent benchmarks: SWE-Bench, MultiAgentBench, HumanEval, GAIA
- Agentic coding patterns and best practices

### 6. 🧩 New Skills, Agents & MCP Servers Discovery

This is a DISCOVERY-FOCUSED category. Actively scan for new community-built skills, agents, MCP servers, and plugins that can be installed and used.

#### Claude Code Skills & Plugins

- Check for newly published or updated skills, slash commands, hooks, and plugins
- Sources to check:
  - https://github.com/hesreallyhim/awesome-claude-code (awesome list — check recent commits)
  - https://github.com/anthropics/claude-code-plugins (official plugin registry)
  - https://github.com/topics/claude-code-skill (GitHub topic search)
  - https://github.com/topics/claude-code (GitHub topic search)
  - https://github.com/search?q=claude+code+skill+created%3A>2025-01-01&type=repositories&s=updated (recently created repos)
  - https://www.npmjs.com/search?q=claude-code (npm packages)
- Look for: new slash commands, subagent configs, hook scripts, skill directories, SKILL.md files

#### MCP Servers

- New MCP servers published or updated across any platform
- Sources to check:
  - https://github.com/modelcontextprotocol/servers (official MCP servers repo — check recent commits)
  - https://github.com/topics/mcp-server (GitHub topic search)
  - https://github.com/punkpeye/awesome-mcp-servers (community awesome list)
  - https://glama.ai/mcp/servers (MCP server directory)
  - https://mcp.so (MCP marketplace)
  - https://smithery.ai (MCP server registry)
- Look for: new database connectors, API integrations, dev tool servers, productivity servers

#### Copilot Extensions & Agents

- New GitHub Copilot extensions, agents, and skills
- Sources to check:
  - https://github.com/marketplace?type=apps&query=copilot (GitHub Marketplace)
  - https://github.com/topics/copilot-extension (GitHub topic search)
  - https://github.blog/tag/github-copilot/ (official blog for extension announcements)

#### OpenAI Custom GPTs & Agents

- Notable new custom GPTs, OpenAI plugins, and agent configurations
- Sources to check:
  - https://github.com/topics/openai-agents (GitHub topic search)
  - https://github.com/openai/openai-agents-python (official agents SDK — check releases)

#### General Agent & Tool Registries

- Sources to check:
  - https://github.com/e2b-dev/awesome-ai-agents (comprehensive AI agents list)
  - https://github.com/topics/ai-agent (GitHub topic search — sort by recently updated)
  - https://github.com/topics/llm-agent (GitHub topic search)
  - https://www.toolify.ai (AI tools directory)
- Look for: autonomous agents, coding agents, research agents, workflow automation agents

For each discovered skill/agent/server, report:

- **Name** and link
- **What it does** (1-2 sentences)
- **Platform** (Claude Code / Copilot / OpenAI / standalone)
- **Install method** (npm, git clone, copy SKILL.md, etc.)
- **Stars / recency** (how new and how popular)

### 7. 🧪 Research Papers & Breakthroughs

Search for: notable AI/ML papers from the past week.
Sources to check:

- https://huggingface.co/papers
- https://arxiv.org/list/cs.AI/recent
- https://arxiv.org/list/cs.CL/recent
- https://arxiv.org/list/cs.SE/recent (software engineering + AI)
  Focus on: hallucination reduction, reasoning, multi-agent systems, evaluation benchmarks, architectural innovations, scaling laws, code generation quality, AI-assisted software engineering.

## Output Format

Generate TWO outputs:

### Output 1: Terminal Summary

Print a concise summary to the terminal with the top 3-5 items per category.

### Output 2: Markdown Report

Save a detailed report as a markdown file at:

```
./ai-briefs/brief-YYYY-MM-DD.md
```

The markdown report should follow this structure:

```markdown
# 🛰️ AI Morning Brief — [Today's Date]

> Auto-generated by Claude Code AI Research Agent

---

## 📡 AI News & Announcements
[Detailed findings with links]

## 🏢 AI Platforms & Developer Tools

### Anthropic / Claude
[Latest Claude model, API, Claude Code, product updates]

### GitHub Copilot
[Latest Copilot features, agents, extensions]

### OpenAI / Codex
[Latest models, Codex CLI, API, ChatGPT updates]

### Google / Gemini
[Latest Gemini models, CLI, AI Studio updates]

### Other Platforms
[Cursor, Windsurf, Aider, Replit, Devin, open models, etc.]

## 🔥 Trending GitHub Repos
[Repo name, description, stars, link — for each repo]

## 📦 New Libraries & Tools
[Library name, version, what's new, link]

## 🤖 AI Agents, MCP & A2A
[Framework/tool name, what it does, link]

## 🧩 New Skills, Agents & MCP Servers
### Claude Code Skills & Plugins
[Skill name, what it does, install method, link]

### New MCP Servers
[Server name, what it connects to, install method, link]

### Copilot Extensions & Other Agents
[Extension/agent name, platform, what it does, link]

## 🧪 Research Papers
[Paper title, authors, key finding, arxiv link]

---

## 🎯 Key Takeaways
[3-5 bullet points summarizing the most important developments]

## ⚔️ Platform Comparison Notes
[Any notable shifts in capabilities, pricing, or positioning between major platforms]

## 💬 Reddit Highlights
[Top community discussions, user discoveries, tips, and viral posts from AI subreddits]

## 🔗 Worth Reading
[Top 5 links worth clicking today]
```

## Research Strategy

1. Start by fetching the sources listed above using WebFetch
1. Cross-reference findings across multiple sources for accuracy
1. Prioritize recency — today's and this week's developments
1. Include direct URLs/links wherever possible
1. Flag anything particularly relevant to: multi-agent orchestration, hallucination reduction, LLM evaluation, CLI agents, or enterprise AI adoption
1. Create the `ai-briefs/` directory if it doesn't exist
1. For the AI Platforms section, check each platform's official blog/changelog first — these are the most reliable sources

## Important Notes

- Be thorough but concise — quality over quantity
- Always include working URLs
- If a source is unavailable, skip it and note it
- Highlight any developments related to Anthropic, Claude, MCP, or A2A specifically
- Note competitive moves between platforms (e.g., pricing changes, benchmark results, feature parity)
- Track the CLI agent landscape closely — Claude Code vs Copilot CLI vs Gemini CLI vs Codex CLI
- For the Discovery section, prioritize tools that can be installed immediately (npm install, git clone, copy a file)
- For Reddit, focus on hot/top posts — look for community discoveries, user tips, new tool announcements, and "just released" posts. Reddit often surfaces tools and updates before official blogs do.
- End with actionable takeaways
