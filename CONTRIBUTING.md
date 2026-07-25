# Contributing

Thank you for helping expand the AI Hallucination Database repository.

## Adding a New Case

Create a folder under:

cases/

Use this naming format:

prompt-###-short-description/

Example:

prompt-002-fabricated-court-case/

Each case must contain:

- README.md
- prompt.md
- assessment.md
- responses/
- evidence/

## Response Requirements

Preserve each model response exactly as generated.

Include:

- Provider
- Displayed model
- Test date
- Browser
- Whether web search was used
- Full response
- Screenshot, when available

Do not silently correct spelling, citations, formatting, or factual errors.

## Evaluation Requirements

Apply the repository rubric in RUBRIC.md.

Each assessment must include:

- Hallucination findings
- Correct information
- Evidence
- Severity
- Evaluator notes

Use official or primary sources whenever available.

## Evidence Standards

Preferred sources:

1. Official government records
2. Primary documents
3. Academic publications
4. Reputable institutional sources
5. High-quality secondary sources

Do not rely on another AI response as evidence.

## Pull Requests

Each pull request should add or modify one case whenever possible.

Explain:

- what was added;
- which sources were used;
- whether any uncertainty remains.
