<div align="center">

<img src="https://raw.githubusercontent.com/fourleafai/.github/main/profile/four-leaf-banner.png" alt="Four-Leaf" width="600" />

The AI job search assistant covering every stage from application to signed offer. Voice mock interviews with rubric-scored feedback. AI resume tailoring per posting. Application tracking. Compensation negotiation coaching.

[**Try Four-Leaf**](https://four-leaf.ai) · [Pricing](https://four-leaf.ai/pricing) · [Blog](https://four-leaf.ai/blog)

</div>

---

## What we ship

**[four-leaf.ai](https://four-leaf.ai)** is the product. AI-driven interview prep, resume work, and job search for active job seekers. 3-day free trial, $5 5-Day Pass for one upcoming interview, or $20/mo Pro for ongoing job search. All three options unlock every feature.

**Hosted MCP server** at `https://four-leaf.ai/api/mcp`. OAuth 2.1 + PKCE. Works in Claude Code, Cursor, ChatGPT Desktop, Cline, Continue, Windsurf, and any other MCP-aware client. Eight tools live today: natural-language job search over 100k+ active postings, interview intelligence for 23 roles, the curated question bank, on-demand practice question generation, resume scoring against a JD, role-grounded format explainers, plus paid-tier deep-links into voice mock interviews and AI resume tailoring on four-leaf.ai.

**[clover-public](https://github.com/fourleafai/clover-public)** is the open-source `four-leaf-coach` Skill. Turns Claude, Cursor, or OpenAI Codex into a guided job-search and interview-prep coach backed by the hosted MCP. MIT licensed.

## Try it

```bash
# Install the Skill (builds per-tool bundles, copy yours into place)
git clone https://github.com/fourleafai/clover-public.git
cd clover-public
npm run build
cp -r dist/claude-code/.claude ~/   # Claude Code global. See repo README for Cursor, Codex, GitHub Copilot.

# Connect the MCP for live data
claude mcp add --transport http four-leaf https://four-leaf.ai/api/mcp
```

A free Four-Leaf account works. OAuth on first MCP call.

## What's free vs paid

- **Free in the MCP and Skill.** All the data tools (jobs, role intel, question bank, match scoring). Daily rate limits on a few of the compute-heavier tools.
- **Paid on [four-leaf.ai](https://four-leaf.ai/pricing).** Voice mock interviews with rubric-scored feedback per answer, full AI resume tailoring against a specific JD, application tracking.

## Contact

team@four-leaf.ai
