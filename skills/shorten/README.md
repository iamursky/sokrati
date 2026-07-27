# Shorten: an agent skill for editing English business writing in a plain, reader-first style

![Chaotic gray lines of text fall into an orange funnel and emerge as neat, even orange rectangles, turning clutter into structured text](/.github/images/cover.webp)

Inspired by **[«Пиши, сокращай 2025»](https://sokratil.ru/)** ("Write, Shorten 2025") by Maxim Ilyahov and Lyudmila Sarycheva.

> This is the English version. Versions for other languages live in the [root README](../../README.md).

## What it does

Give Claude, ChatGPT, or Codex a piece of business writing in English, such as an email, landing page, press release, resume, report, deck, or cold email. The skill edits it across five levels:

1. **Word-level cleanup** — removes filler phrases, vague wording, inflated vocabulary, empty judgments, and clichés
2. **Sentence-level clarity** — turns nominalizations into verbs, breaks up overloaded sentences, tightens paragraph discipline
3. **Fighting bureaucratese** — six moves against the stilted style of corporate and government documents
4. **Structure and purpose** — checks the useful action, audience, structure, intro, and conclusion
5. **Genre rules** — templates and checks for "about" pages, resumes, cold emails, press releases, work documents, slides, and landing pages

The skill returns an edited version with a change log and recommendations for what to add (facts, examples, research).

## Installation

### Via `npx skills` (recommended)

```bash
npx skills add iamursky/sokrati/tree/main/skills/shorten
```

### ChatGPT

1. Download the entire `skills/shorten` folder, including `SKILL.md` and `references/`
2. In the ChatGPT sidebar, open **Plugins → Skills**
3. Select **Create → Upload from your computer** and upload the skill folder
4. Wait for ChatGPT to finish scanning the skill, then select it with `@` or ask ChatGPT to improve a piece of business writing

### Claude Desktop / Web

1. Download the entire `skills/shorten` folder, including [SKILL.md](SKILL.md) and `references/`
2. Go to **Customize → Skills → + → Upload a skill**
3. Upload the skill folder
4. The skill activates automatically — ask Claude to cut the fluff or make a text "stronger"

### Manual install for Claude Code

```bash
# Personal (available across all projects)
git clone https://github.com/iamursky/sokrati ~/sokrati
ln -s ~/sokrati/skills/shorten ~/.claude/skills/shorten

# Per-project (shared with the team via git)
git clone https://github.com/iamursky/sokrati .sokrati
ln -s .sokrati/skills/shorten .claude/skills/shorten
```

## How to use

The skill triggers automatically when you:

- Ask Claude, ChatGPT, or Codex to edit, review, clean up, or improve any business text in English
- Mention "information style", "infostyle", "Ilyahov", "Glavred", "filler words", or "bureaucratese"
- Ask the assistant to cut the fluff, kill the clichés, or rewrite in "plain language"

### Examples

**Full edit:**

> Edit this landing page copy in plain style: [text]

**Review without rewriting:**

> Give me feedback on this email. What can be improved? [text]

**Question about technique:**

> How should I write an "About us" section?

## Authorship

The skill is inspired by **«Пиши, сокращай 2025»** by Maxim Ilyahov and Lyudmila Sarycheva. It is not an official product of the book's authors and does not reproduce the original text. The ideas and techniques belong to the authors; this skill is one interpretation of those ideas as an agent workflow. If you read Russian and like the book, support the authors by buying it at the link above.
