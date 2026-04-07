# Skill Catalog

This catalog lists all skills currently included in this repository.

## Summary

- Total skills: 7
- Text-based skills: 4
- JavaScript skills: 3
- Skills requiring secrets: 3

## Skills

| Skill | Folder | Type | Requires Secret | Description |
| --- | --- | --- | --- | --- |
| Fire Service Advisor | [skills/fire-service-advisor](skills/fire-service-advisor) | Text | No | Emergency triage, tactical decision support, and incident command guidance for fire-related incidents. |
| Gemini Search | [skills/gemini-search](skills/gemini-search) | JavaScript | Yes | Live web search via Gemini grounding with synthesized answers and sources. |
| Legal Service Advisor | [skills/legal-service-advisor](skills/legal-service-advisor) | Text | No | Legal issue spotting and structured guidance across major legal domains. |
| Mood Music | [skills/mood-music](skills/mood-music) | JavaScript | Yes | Mood-based music generation workflow with Loudly API integration. |
| Personal Finance Coach | [skills/personal-finance-coach](skills/personal-finance-coach) | Text | No | Practical budgeting, savings, debt payoff, and 30-day personal finance action planning. |
| Restaurant Roulette | [skills/restaurant-roulette](skills/restaurant-roulette) | JavaScript | Yes | Interactive restaurant roulette wheel based on cuisine and location. |
| Sports Playbook | [skills/sports-playbook](skills/sports-playbook) | Text | No | Coaching-focused game analysis, matchup optimization, and play planning. |

## Skill File Entry Points

- Fire Service Advisor: [skills/fire-service-advisor/SKILL.md](skills/fire-service-advisor/SKILL.md)
- Gemini Search: [skills/gemini-search/SKILL.md](skills/gemini-search/SKILL.md), [skills/gemini-search/scripts/index.html](skills/gemini-search/scripts/index.html)
- Legal Service Advisor: [skills/legal-service-advisor/SKILL.md](skills/legal-service-advisor/SKILL.md)
- Mood Music: [skills/mood-music/SKILL.md](skills/mood-music/SKILL.md), [skills/mood-music/scripts/index.html](skills/mood-music/scripts/index.html)
- Personal Finance Coach: [skills/personal-finance-coach/SKILL.md](skills/personal-finance-coach/SKILL.md)
- Restaurant Roulette: [skills/restaurant-roulette/SKILL.md](skills/restaurant-roulette/SKILL.md), [skills/restaurant-roulette/scripts/index.html](skills/restaurant-roulette/scripts/index.html)
- Sports Playbook: [skills/sports-playbook/SKILL.md](skills/sports-playbook/SKILL.md)

## Notes

- Skill metadata is defined in each `SKILL.md` frontmatter.
- JavaScript skills run in a sandboxed hidden webview through `scripts/index.html`.
- Secret requirements are enforced via `metadata.require-secret`.
