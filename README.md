# Resume Checker for Claude

**Free AI-powered resume scoring for Claude Code and Cowork.** Get instant feedback on your resume with a 0-100 score and actionable fixes.

[![Claude Plugin](https://img.shields.io/badge/Claude-Plugin-blueviolet)](https://claude.ai)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## What It Does

Drop any resume (PDF, DOCX, or paste text) and get:

- **0-100 Score** — Weighted across 6 categories
- **Top 3-5 Issues** — Prioritized fixes that matter most
- **ATS Compatibility Check** — Will your resume parse correctly?
- **Weak Verb Detection** — Flags "Responsible for," "Helped," "Assisted"
- **Role-Specific Tips** — Tailored advice for engineering, product, marketing, sales, design, and ops

---

## Quick Start

### Install in Claude Code
```bash
claude plugin add resume-checker-claude
```

### Install in Cowork
1. Download this repo
2. In Cowork, go to **Settings → Plugins → Add Plugin**
3. Select the downloaded folder

---

## Commands

| Command | Description |
|---------|-------------|
| `/resume-score` | Score any resume with detailed breakdown |
| `/resume-tips` | Get role-specific resume best practices |

---

## Scoring Breakdown

| Category | Points | What It Checks |
|----------|--------|----------------|
| **Contact Info** | 10 | Name, email, phone, LinkedIn, portfolio |
| **Sections** | 12 | Experience, education, skills, summary |
| **Work History** | 8 | Timeline, dates, bullet count |
| **Skills** | 15 | Core skill coverage, quantity |
| **Impact** | 40 | Metrics, action verbs, specificity |
| **Language** | 15 | Weak phrases, repetition, grammar |

**Calibration:** 40-60 = typical first upload. 70+ = strong. 85+ = excellent.

---

## Example Output

```
Resume Score: 67/100

Top Issues:
1. ⚠️ 4 bullets start with "Responsible for" — shows observation, not ownership
2. ⚠️ Missing metrics in 6 bullets — add numbers to prove impact  
3. ⚠️ Only 6 skills listed — aim for 10-15 relevant skills
4. ℹ️ No LinkedIn URL — add it to contact section

Quick Wins:
→ Replace "Responsible for managing" with "Managed" or "Led"
→ Add one metric per bullet: %, $, time saved, team size
```

---

## Role-Specific Tips

Run `/resume-tips [role]` for targeted advice:

**Software Engineer**
- Lead with technical impact, not tasks
- Include specific technologies with versions
- Show scale: requests/sec, data size, uptime %

**Product Manager**
- Lead with business outcomes, not activities
- Show tradeoff decisions you made
- Quantify: DAU, conversion, retention, revenue

**Marketing**
- Lead with pipeline and revenue impact
- Include CAC, conversion rates, growth %
- Show both strategy and execution

**Sales**
- Lead with quota attainment and deal size
- Show progression: AE → Sr AE → Enterprise
- Include outbound metrics if relevant

---

## Why This Exists

Most resume feedback is generic. This skill applies the same scoring logic used by [Soared](https://soared.ai), an AI resume tailoring tool that helps job seekers optimize for specific roles.

**What makes it different:**
- Scores like a recruiter (6 seconds of attention)
- Catches weak verbs that signal "I watched" vs "I did"
- Role-aware (PM resume ≠ SWE resume)
- ATS-focused (will it parse correctly?)

---

## Roadmap

- [x] Resume scoring skill
- [x] Role-specific tips command
- [ ] Job description matching (`/resume-match`)
- [ ] AI-powered tailoring (`/resume-tailor`)
- [ ] Cover letter generation (`/cover-letter`)

---

## Contributing

PRs welcome. If you find edge cases the scorer misses, open an issue with the resume text (anonymized).

---

## License

MIT — use it, fork it, improve it.

---

## Links

- [Soared](https://soared.ai) — Full resume tailoring platform
- [Claude Plugins Docs](https://docs.anthropic.com/plugins)
- [Report Issues](https://github.com/soared-ai/resume-checker-claude/issues)

---

**Built for job seekers who want real feedback, not platitudes.**