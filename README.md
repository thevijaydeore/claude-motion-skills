# claude-motion-skills

Skills for Claude to generate SaaS product launch videos — no footage needed.

## Skills

| Skill | What it does |
|---|---|
| [`launch-director`](launch-director/SKILL.md) | Interviews you across 8 stages and outputs a complete MASTERPLAN + BUILD command for your launch video. |
| [`explainer-default`](explainer-default/README.md) | Clean 45–90 s product demo: your UI rebuilt and filmed up close. |
| [`explainer-high-energy`](explainer-high-energy/README.md) | 12–20 s beat-locked kinetic hype promo. |
| [`explainer-engaging`](explainer-engaging/README.md) | 10–30 s one-take story: one element travels through your product's workflow. |
| [`sound-effects`](sound-effects/README.md) | Adds real CC0 sound effects timed to the beat at −16 LUFS. |

## How it works

1. Start with the **launch-director** skill — it runs a structured interview (product, message, features, brand, style, format) and auto-installs the other skills.
2. It outputs a **MASTERPLAN** with a one-line BUILD command.
3. Run BUILD → Claude renders the draft MP4.
4. Sound effects are added automatically in the final step.

## Install

```bash
npx skills add thevijaydeore/claude-motion-skills
```

Or manually: clone this repo and copy the skill folders into `.claude/skills/`.

## Requirements

- Node 18+
- Python 3.10+
- ffmpeg
- Playwright (installed automatically by the skills)

## Attribution

The `explainer-*` and `sound-effects` skills are adapted from [Barty-Bart/motion-graphics](https://github.com/Barty-Bart/motion-graphics) (MIT License — Copyright © 2026 Bart). See [LICENSE-upstream](LICENSE-upstream) for the original terms.

The `launch-director` skill is original work by [Dhumi Inc](https://dhumi.com).

## License

MIT — see [LICENSE](LICENSE).
