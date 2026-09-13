# Anti-AI-Slop Writing Skill

A Claude Code skill (and a portable SKILL.md) that makes an AI write like a person, by banning the vocabulary, sentence rhythm, punctuation habits and formatting tics that readers and detection tools flag as machine-written.

## What It Does

Anything the AI writes for you — a tweet, an email, an article, a bio, a report, a bit of landing-page copy — gets filtered through a set of hard constraints before it reaches you.

The rules come from research by Carnegie Mellon (2025), Wikipedia's *Signs of AI Writing* page, Buffer's analysis of 52M posts, and detection patterns people have catalogued on X and Reddit.

## What It Catches

- **53 banned words** flagged across several AI-detection studies: delve, tapestry, landscape, testament, vibrant, pivotal and the rest of that crowd
- **36 banned phrases** — "In today's competitive...", "It's worth noting...", "Not just X, but Y"
- **16 banned sentence openers** such as "Certainly," "Moreover," and "Additionally,"
- **11 structural patterns**: the rule of three, uniform sentence length, parataxis, the hedging seesaw, corporate pep talk, passive voice
- **Punctuation tells** — em dash overuse, exclamation spam, ellipsis abuse
- **Formatting leaks** like markdown in plain-text contexts, emoji bullets, hashtag stacks
- **Accuracy failures**: invented statistics, fabricated quotes, fake anecdotes

Plus a per-model list of first-word tells, because ChatGPT, Claude, Grok, Gemini and DeepSeek each open a response in their own predictable way.

## Installation

### Claude Code (plugin marketplace)

```
/plugin marketplace add obi12341/anti-ai-slop-writing
/plugin install anti-ai-slop-writing@anti-ai-slop
```

### Claude Code (manual)

Copy the skill folder into your personal skills directory:

```bash
git clone https://github.com/obi12341/anti-ai-slop-writing.git
cp -r anti-ai-slop-writing/skills/anti-ai-slop-writing ~/.claude/skills/
```

For a single project instead, copy it to `.claude/skills/` in that repo.

### Other AI tools (Cursor, Codex, Gemini CLI, etc.)

Copy `skills/anti-ai-slop-writing/` into your tool's skills directory. Keep the `references/` folder next to `SKILL.md`; the skill loads the banned-words list from there on demand.

### Any AI chat (ChatGPT, Claude.ai, Gemini, etc.)

Paste the contents of `SKILL.md` and `references/banned-words.md` at the start of the conversation. It works as a system-level writing constraint.

## Usage

The skill fires on its own when you ask for writing. To force it:

```
/anti-ai-slop-writing
```

Installed as a plugin it also answers to `/anti-ai-slop-writing:anti-ai-slop-writing` if another command has already claimed the short name.

Or just ask: "write this email and make it sound human."

## Repository Layout

```
.
├── .claude-plugin/
│   ├── marketplace.json              # marketplace manifest (/plugin marketplace add)
│   └── plugin.json                   # plugin metadata
└── skills/
    └── anti-ai-slop-writing/
        ├── SKILL.md                  # core rules, always loaded
        └── references/
            └── banned-words.md       # full banned vocabulary, loaded on demand
```

The repository root doubles as the plugin root, so the marketplace entry points at `./` and Claude Code picks up `skills/` from there.

## Author

Created by [Jalaaldeen](https://x.com/jalaal_tweets), builder of Wardex, ZakatChain, and open-source AI tooling for founders. This repository packages the skill as an installable Claude Code plugin and adds the parataxis rule.

## License

MIT
