# Gemma Skills for AI Edge Gallery

This repository contains useful skills for Gemma 4 in Google AI Edge Gallery.

The goal is simple: give on-device mobile LLMs practical capabilities through reusable skill packages that are easy to install, test, and extend.

## What This Project Provides

- Curated skills for real-world use cases such as legal guidance, coaching, recommendations, and web-grounded search
- Support for both skill types used by AI Edge Gallery:
	- Text-based skills (SKILL.md only)
	- JavaScript skills (SKILL.md plus scripts/index.html running in a sandboxed hidden webview)
- A structure that is easy to contribute to and review

## Disclaimer

These skills are provided for demonstration and educational purposes only.

They are intended to showcase implementation patterns and practical possibilities for Gemma 4 in Google AI Edge Gallery. Actual behavior, quality, and outputs may differ based on model version, platform implementation, device environment, and runtime configuration.

Do not treat these skills as guarantees of identical behavior across systems. **Always validate and test thoroughly in your own environment before relying on any skill for critical, safety-sensitive, legal, financial, medical, or production use.**

## Skill Format

Each skill lives in its own folder and follows one of these patterns:

1. Text-based skill
	 - SKILL.md

2. JavaScript skill
	 - SKILL.md
	 - scripts/index.html
	 - Optional assets/ for webviews and UI files

## Available Skills

The complete and up-to-date list is maintained in [CATALOG.md](CATALOG.md).

| Skill | Folder | Type | Requires Secret | Description |
| --- | --- | --- | --- | --- |
| Fire Service Advisor | [skills/fire-service-advisor](skills/fire-service-advisor) | Text | No | Emergency triage, tactical decision support, and incident command guidance for fire-related incidents. |
| Gemini Search | [skills/gemini-search](skills/gemini-search) | JavaScript | Yes | Live web search via Gemini grounding with synthesized answers and sources. |
| Legal Service Advisor | [skills/legal-service-advisor](skills/legal-service-advisor) | Text | No | Legal issue spotting and structured guidance across major legal domains. |
| Mood Music | [skills/mood-music](skills/mood-music) | JavaScript | Yes | Mood-based music generation workflow with Loudly API integration. |
| Personal Finance Coach | [skills/personal-finance-coach](skills/personal-finance-coach) | Text | No | Practical budgeting, savings, debt payoff, and 30-day personal finance action planning. |
| Restaurant Roulette | [skills/restaurant-roulette](skills/restaurant-roulette) | JavaScript | Yes | Interactive restaurant roulette wheel based on cuisine and location. |
| Sports Playbook | [skills/sports-playbook](skills/sports-playbook) | Text | No | Coaching-focused game analysis, matchup optimization, and play planning. |

For detailed metadata (type, secret requirement, folder links, and entry points), see [CATALOG.md](CATALOG.md).

## Getting Started

1. Pick a skill folder under skills/.
2. Review its SKILL.md and README.md.
3. Import SKILL.md into Google AI Edge Gallery using URL or local file.
4. If required, provide a secret key when the app prompts for it.

For implementation details and full skill architecture, see SKILL-GUIDE.md.

## Contributing

Contributions are welcome for new skills and improvements to existing ones.

Recommended workflow:

1. Create a new folder under skills/ using kebab-case.
2. Add SKILL.md with clear metadata and activation description.
3. For JS skills, add scripts/index.html and keep logic sandbox-safe.
4. Add a README.md with overview, installation, and usage examples.
5. Validate behavior in AI Edge Gallery before opening a PR.

## Design Principles

- Keep skills useful and domain-specific
- Prefer text-only skills unless JavaScript adds clear value
- Keep JavaScript lightweight and webview-safe
- Avoid hardcoding secrets
- Return structured outputs and clear errors

## License

This project is licensed under the Apache License, Version 2.0. See LICENSE for details.
