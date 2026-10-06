# ADS-STE100 Rewrite & Maintain Voice/Tone

A ChatGPT and Codex skill for rewriting arbitrary prose while preserving the author's meaning, voice, and tone by default. Built for everyday writing, emails, articles, stories, speeches, marketing, and persuasive copy.

Adapted from [danyuchn/asd-ste100-skill](https://github.com/danyuchn/asd-ste100-skill). It carries over the original's attention to clarity, ambiguity, and faithful meaning, with flexible editorial guidance for writing where personality and persuasion matter.

**[Download skill.zip](https://github.com/joshuaoxlee/ads-ste100-rewrite-maintain-voice-tone/releases/latest/download/skill.zip)** · [Read the skill](clear-rewrite/SKILL.md) · [See editing examples](clear-rewrite/references/examples.md)

## What it does

- Preserves the author's voice unless you ask for a change.
- Rewrites, polishes, simplifies, tightens, or adapts supplied prose to a different audience, tone, or channel.
- Supports persuasive copy, including hooks, benefits, and calls to action, without inventing proof or changing offer terms.
- Protects facts, uncertainty, conditions, commitments, quotations, links, and template variables.
- Returns a ready-to-use rewrite by default, with explanations or comparisons when requested.
- Leaves effective writing unchanged when an edit would not improve it.

Sentence length, punctuation, tense, idioms, metaphor, and repetition are editorial choices. There is no universal word cap or automatic ban on marketing language.

## Use the skill

Download the ZIP for a host that supports skill bundles, or use the `clear-rewrite` folder directly. The bundle contains one skill and its supporting references. It needs no scripts, credentials, connectors, or network access to rewrite supplied text.

For a local Codex installation, place the extracted `clear-rewrite` folder in your personal skills directory, typically `~/.codex/skills/`. If `CODEX_HOME` is set, use `$CODEX_HOME/skills/` instead. The installed skill's identifier is `clear-rewrite`.

Select the skill in your host, or invoke it in Codex with `$clear-rewrite`, and include the passage to edit. For example:

> Use $clear-rewrite to polish this email. Keep it warm and conversational: [paste text]

> Use $clear-rewrite to make this landing-page copy more persuasive. Preserve the brand voice and all offer conditions: [paste text]

> Use $clear-rewrite to put this in plain language without changing what is required or optional: [paste text]

> Use $clear-rewrite to shorten this to 150 words. Keep the humour and flag any material detail that cannot fit: [paste text]

You can also ask for a more formal or playful tone, a different audience, a before-and-after comparison, or multiple alternatives. Without further direction, it makes a moderate clarity edit and preserves the source voice, language, format, and level of detail.

## Example

**Request:** Make this clearer.

**Before:**

> Hey Sam, just popping in because I wanted to see if you might have had a chance to look at the draft I sent over last week? No rush at all — Friday is still totally fine.

**After:**

> Hey Sam, just checking whether you've had a chance to look at the draft I sent last week. No rush — Friday is still totally fine.

The wording is tighter; the warmth and timing remain. More examples cover qualified offers, sales copy, literary voice, ambiguity, and functional text.

## Package contents

```text
clear-rewrite/
├── SKILL.md
├── LICENSE
├── agents/
│   └── openai.yaml
└── references/
    ├── examples.md
    ├── origin.md
    └── persuasive-copy.md
```

## Source and license

The adaptation is based on upstream revision [`32511c6`](https://github.com/danyuchn/asd-ste100-skill/tree/32511c6992ecb5f1971e46a2943f2e6adceedafe). See the [source and adaptation notes](clear-rewrite/references/origin.md) for the changes in scope.

Distributed under the [MIT License](LICENSE), with the original copyright notice for Dustin Yuchen Teng preserved. This skill is inspired by ASD-STE100 clarity principles. It does not reproduce the official dictionary or standard, certify compliance, or imply endorsement by ASD or the upstream author.
