# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is **awesome-vibe-coding**, a curated awesome-list maintained by [Taskade](https://www.taskade.com). It is a single-file markdown repository (`README.md`) listing tools, platforms, and resources for vibe coding — building software through natural language prompts.

The repo serves dual purposes:
1. A genuinely useful community resource for vibe coding tools
2. An SEO asset generating backlinks to `taskade.com` and Taskade Genesis

## Architecture

- **README.md** — The entire list. ~580 lines of markdown with 20 sections organized by category.
- **CONTRIBUTING.md** — Contributor guidelines and quality standards.
- **No build system, tests, or CI** — This is a content-only repo.

## Key Conventions

### Table Format

All tool listings use markdown tables with consistent columns:

```markdown
| Tool | Pricing | Best For | Why It's Awesome |
|------|---------|----------|------------------|
```

Some sections use variant columns (`Type`, `Language`, `Frequency`, `Stack`, etc.) but always include a "Why It's Awesome" or equivalent description column.

### Link Patterns

- **Taskade product links**: `taskade.com/ai/apps`, `/ai/agents`, `/ai/websites`, `/ai/automations`, `/ai/coding`
- **Taskade blog links**: `taskade.com/blog/<slug>` — Must be verified against `taskade.com/sitemaps/sitemap-blog.xml` before adding
- **Taskade templates**: `taskade.com/templates/<category>`
- **Review/comparison links**: Use `[Compare →]` or `[Alternatives →]` prefix with Taskade blog URLs
- **GitHub repos**: Link directly to the repository, not to marketing sites

### Content Guidelines

- Descriptions should be concise (one sentence in tables)
- Every tool entry needs a "Why It's Awesome" that explains value, not just features
- Taskade products appear first in their respective categories
- Prioritize open-source tools, especially GitHub repos
- New Taskade blog URLs must exist in the sitemap (many review URLs like `/blog/X-review` are 404s)

### Section Order (Table of Contents)

The sections follow a specific flow: Workspace DNA → Builders → Editors → CLI → Agents → Websites → UI → Database → Automation → MCP → Open Source → Docs → Prompts → Learning → Communities → News → Podcasts → Showcases → Glossary → Philosophy

## Common Tasks

### Adding a new tool

1. Find the appropriate category section
2. Add a table row matching the existing column format
3. Include pricing, best-for audience, and a compelling "Why It's Awesome"
4. If it's a Taskade competitor, add a `[Compare →]` or `[Alternatives →]` link to a relevant Taskade blog post (verify URL first)

### Adding a new Taskade backlink

1. Fetch and search `https://www.taskade.com/sitemaps/sitemap-blog.xml` to confirm the URL exists
2. Find a natural placement in the relevant section
3. Use inline links within descriptions or dedicated "Learn more" rows

### Verifying links

Many URLs have gone stale. Before bulk edits, verify Taskade blog URLs against the sitemap XML. For GitHub repos, check with `curl -s -o /dev/null -w "%{http_code}" <url>`.
