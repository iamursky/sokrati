# Sokrati: an agent skill for editing business writing in plain, reader-first style

[![skills.sh](https://skills.sh/b/iamursky/sokrati)](https://skills.sh/iamursky/sokrati)

![Chaotic gray lines of text fall into an orange funnel and emerge as neat, even orange rectangles, turning clutter into structured text](/.github/images/cover.webp)

Inspired by **[«Пиши, сокращай 2025»](https://sokratil.ru/)** ("Write, Shorten 2025") by Maxim Ilyahov and Lyudmila Sarycheva — a Russian-language classic on business writing that maps well onto plain-writing traditions in other languages.

## What it does

Give Claude, ChatGPT, or Codex a piece of business writing, such as an email, landing page, press release, resume, report, deck, or cold email. The skill edits it across five levels:

1. **Word-level cleanup** — removes filler phrases, vague wording, inflated vocabulary, empty judgments, and clichés
2. **Sentence-level clarity** — turns nominalizations into verbs, breaks up overloaded sentences, tightens paragraph discipline
3. **Fighting bureaucratese** — six moves against the stilted style of corporate and government documents
4. **Structure and purpose** — checks the useful action, audience, structure, intro, and conclusion
5. **Genre rules** — templates and checks for "about" pages, resumes, cold emails, press releases, work documents, slides, and landing pages

The skill returns an edited version with a change log and recommendations for what the author should add (facts, examples, research).

## Language versions

Each language has its own adapted version — native filler phrases, native clichés, native examples — not a translation.

| Language | Skill name | Folder                               |
| -------- | ---------- | ------------------------------------ |
| Русский  | `sokrati`  | [skills/sokrati/](skills/sokrati/)   |
| English  | `shorten`  | [skills/shorten/](skills/shorten/)   |
| Català   | `escurca`  | [skills/escurca/](skills/escurca/)   |
| Deutsch  | `kuerzen`  | [skills/kuerzen/](skills/kuerzen/)   |
| Español  | `abrevia`  | [skills/abrevia/](skills/abrevia/)   |
| Français | `abrege`   | [skills/abrege/](skills/abrege/)     |
| Italiano | `abbrevia` | [skills/abbrevia/](skills/abbrevia/) |

Each folder has its own `README.md`, `SKILL.md`, and `references/KNOWLEDGE.md`.

## Installation

### Via `npx skills` (recommended)

```bash
# One skill (replace shorten with your target language's skill name)
npx skills add iamursky/sokrati/tree/main/skills/shorten

# All seven languages at once
npx skills add iamursky/sokrati
```

### ChatGPT

1. Download the folder for your target language, including `SKILL.md` and `references/`
2. In the ChatGPT sidebar, open **Plugins → Skills**
3. Select **Create → Upload from your computer** and upload the skill folder
4. Wait for ChatGPT to finish scanning the skill, then select it with `@` or ask ChatGPT to improve business writing in that language

### Claude Desktop / Web

1. Download the folder for your target language, including `SKILL.md` and `references/`
2. Go to **Customize → Skills → + → Upload a skill**
3. Upload the skill folder
4. The skill activates automatically when you ask Claude to clean up, tighten, or improve business writing in that language

### Manual install for Claude Code

```bash
# Personal (any language, example: English)
git clone https://github.com/iamursky/sokrati ~/sokrati
ln -s ~/sokrati/skills/shorten ~/.claude/skills/shorten

# Per-project (shared via git)
git clone https://github.com/iamursky/sokrati .sokrati
ln -s .sokrati/skills/shorten .claude/skills/shorten
```

Each language ships as a separate skill — you can install several side by side without conflict, since each has its own name in the frontmatter.

## How it activates

The skill triggers automatically when you:

- Ask Claude, ChatGPT, or Codex to edit, review, clean up, or improve any business text
- Mention "information style", "infostyle", "Ilyahov", "Glavred", "filler words", or "bureaucratese" (or the local equivalents)
- Ask the assistant to cut the fluff, kill the clichés, or rewrite in "plain language"

## Authorship

The skill is inspired by **«Пиши, сокращай 2025»** by Maxim Ilyahov and Lyudmila Sarycheva. It is not an official product of the book's authors and does not reproduce the original text. The ideas and techniques belong to the authors; this skill is one interpretation of those ideas as an agent workflow. If you read Russian and like the book, support the authors by buying it at the link above.

## License

See [license](license).
