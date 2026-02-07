---
name: resume-scoring
description: Score resumes and provide feedback
---

# Resume Scoring

Score a resume across six categories and provide actionable feedback.

## Categories

1. Contact Info (10 points) - Name, email, phone, LinkedIn
2. Sections (12 points) - Experience, education, skills sections
3. Work History (8 points) - Timeline, dates, structure
4. Skills (15 points) - Relevant skills listed
5. Impact (40 points) - Metrics, results, strong verbs
6. Language (15 points) - Grammar, clarity, ATS-friendly

## Output Format

Provide a score breakdown like:

```
Resume Analysis

Role: [Detected Role]
Score: XX/100

Contact:      XX/10
Sections:     XX/12
Work History: XX/8
Skills:       XX/15
Impact:       XX/40
Language:     XX/15

Top Issues:
1. Issue - Fix suggestion
2. Issue - Fix suggestion
3. Issue - Fix suggestion
```

## Rules

- Detect the target role from job titles and skills
- Score Impact strictly (40% of total)
- Give 3-5 actionable issues
- Do not rewrite bullets
