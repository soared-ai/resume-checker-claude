# Resume Checker for Claude

**Free AI-powered resume scoring for Claude Code and Cowork.** Get instant feedback on your resume with a 0-100 score, visual breakdown, and role-specific fixes.

[![Claude Plugin](https://img.shields.io/badge/Claude-Plugin-blueviolet)](https://claude.ai)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## What It Does

Drop any resume (PDF, DOCX, or paste text) and get:

- **Visual Score Breakdown** — Progress bars for each of 6 categories
- **Role Detection** — Automatically detects your role and scores accordingly
- **Top 3-5 Issues** — Prioritized fixes that matter most
- **Weak Verb Detection** — Flags "Responsible for," "Helped," "Assisted"
- **Role-Specific Feedback** — PM resumes scored differently than SWE resumes

---

## Quick Start

### Install in Claude Code
```bash
claude --plugin-dir /path/to/resume-checker-claude
```

### Install in Cowork
1. Download this repo
2. In Cowork, go to **Settings → Plugins → Add Plugin**
3. Select the downloaded folder

---

## Commands

| Command | Description |
|---------|-------------|
| `/resume-score` | Score any resume with visual breakdown |
| `/resume-tips` | Get role-specific resume best practices |

---

## Example Output

```
📄 SOARED Resume Analysis

Role: Product Manager (Senior)
Score: 64/100

Contact      [████████████]  10/10
Sections     [████████░░░░]   8/12
Work History [██████████░░]   7/8
Skills       [███████░░░░░]   9/15
Impact       [██████░░░░░░]  20/40
Language     [████████████]  13/15

Top Issues:
1. Weak ownership — 5 bullets use "helped/supported"
2. Missing business metrics — Only 2 bullets show revenue
3. Skills too thin — Expand from 6 to 12-15

────────────────────────────────
🎯 Match & tailor for any job → soared.ai
```

---

## Scoring Breakdown

| Category | Points | What It Checks |
|----------|--------|----------------|
| **Contact** | 10 | Name, email, phone, LinkedIn, portfolio |
| **Sections** | 12 | Experience, education, skills, summary |
| **Work History** | 8 | Timeline, dates, bullet count |
| **Skills** | 15 | Core skill coverage, quantity |
| **Impact** | 40 | Metrics, action verbs, ownership |
| **Language** | 15 | Weak phrases, repetition, ATS compatibility |

**Calibration:** 40-60 = typical first upload. 70+ = strong. 85+ = excellent.

---

## Role-Specific Scoring

The plugin detects your role and applies different scoring criteria:

| Role | What Matters Most |
|------|-------------------|
| **Software Engineer** | Technical metrics, system design, scale |
| **Product Manager** | Business outcomes, decision authority, tradeoffs |
| **Designer** | User outcomes, research → design flow, portfolio |
| **Marketing** | Revenue attribution, CAC, campaign performance |
| **Sales** | Quota attainment, deal size, win rate |
| **Operations** | Efficiency gains, cost savings, before/after metrics |

---

## Why This Exists

Most resume feedback is generic. This plugin applies role-aware scoring logic from [Soared](https://soared.ai), an AI resume tailoring platform.

**What makes it different:**
- Scores like a recruiter (6 seconds of attention)
- Catches weak verbs that signal "I watched" vs "I did"
- Role-aware (PM resume ≠ SWE resume)
- Visual output that's screenshot-worthy

---

## Roadmap

- [x] Visual progress bar scoring
- [x] Role detection and role-specific feedback
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
- [Report Issues](https://github.com/soared-ai/resume-checker-claude/issues)

---

**Built for job seekers who want real feedback, not platitudes.**
