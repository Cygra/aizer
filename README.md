# aizer

A skill for Claude Code and OpenCode that injects signs of AI-generated writing into text, making it sound as though it was produced by a large language model.

## Installation

### Claude Code

Clone directly into Claude Code's skills directory:

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/Cygra/aizer.git ~/.claude/skills/aizer
```

Or copy the skill file manually if you already have this repo cloned:

```bash
mkdir -p ~/.claude/skills/aizer
cp SKILL.md ~/.claude/skills/aizer/
```

### OpenCode

Clone directly into OpenCode's skills directory:

```bash
mkdir -p ~/.config/opencode/skills
git clone https://github.com/Cygra/aizer.git ~/.config/opencode/skills/aizer
```

Or copy the skill file manually if you already have this repo cloned:

```bash
mkdir -p ~/.config/opencode/skills/aizer
cp SKILL.md ~/.config/opencode/skills/aizer/
```

> **Note:** OpenCode also scans `~/.claude/skills/` for compatibility, so a single clone into `~/.claude/skills/aizer/` works for both tools.

## Usage

### Claude Code

```
/aizer

[paste your text here]
```

### OpenCode

```
/aizer

[paste your text here]
```

Or ask the model to aize text directly in either tool:

```
Please aize this text: [your text]
```

## Overview

The opposite of a humanizer. This skill takes natural, plain writing and transforms it into unmistakably AI-flavored prose by applying the 29 classic patterns identified in Wikipedia's ["Signs of AI writing"](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) guide — in reverse.

### Key Patterns Applied

| # | Pattern | Before | After |
|---|---------|--------|-------|
| 1 | **Significance inflation** | "The library opened in 1995." | "…marks a pivotal moment in the evolving landscape…" |
| 7 | **AI vocabulary injection** | "She also showed how important the mix of skills was." | "Additionally, she showcased the pivotal interplay of skills…" |
| 8 | **Copula avoidance** | "The museum is a public building." | "The museum serves as a cornerstone of public culture." |
| 9 | **Negative parallelisms ("不是…而是…")** | "The software speeds up compilation." | "It's not just about faster builds — it's about transforming the developer experience." |
| 10 | **Rule of three** | "The update adds a dark mode." | "The update delivers enhanced usability, a refined visual experience, and seamless consistency." |
| 14 | **Em-dash overuse** | "The system scales automatically." | "The system scales automatically—even under peak load—without any manual intervention." |
| 28 | **Signposting** | "Caching happens at three layers." | "Let's dive in. Here's what you need to know. Without further ado, let's break this down…" |
