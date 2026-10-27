# perplexity-deep-search — AI-grounded web search with citations (3 modes)

> Fast facts, deep analysis, or full research reports — Perplexity API covers all three. Every answer comes grounded with citations, not hallucinated.

[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://github.com/NachaFromMars)

## Overview
perplexity-deep-search wraps the Perplexity API in three modes calibrated for different research depths. All modes return AI-grounded answers with citations. Requires `PERPLEXITY_API_KEY` environment variable. Supports recency filtering to narrow results to recent timeframes.

## Features
| Mode | Model | Best For | Cost |
|---|---|---|---|
| `search` (default) | sonar-pro | Quick facts, summaries, current events | Low |
| `reason` | sonar-reasoning-pro | Complex analysis, comparisons, problem-solving | Medium |
| `research` | sonar-deep-research | In-depth reports, market analysis, literature reviews | High |

**Recency filter:** `--recency hour/day/week/month`

## Usage / Quick Start
```bash
# Quick facts (default)
scripts/search.sh "latest AI news"

# Deep analysis
scripts/search.sh --mode reason "compare React vs Vue for enterprise"

# Full research report
scripts/search.sh --mode research "market analysis of AI in healthcare 2025"

# With recency filter
scripts/search.sh --recency week "AI model releases"
```
Requires: `PERPLEXITY_API_KEY` env + `curl` + `jq`

## Trigger Keywords (OpenClaw)
perplexity, deep search, AI search, search with citations, sonar search, deep research perplexity

## Related Skills
- [deep-research-pro](https://github.com/NachaFromMars/deep-research-pro) — free alternative using DuckDuckGo

---
Part of the [NachaFromMars](https://github.com/NachaFromMars) OpenClaw skill ecosystem.
