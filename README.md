# AI Hallucination Database

An evidence-backed database of factual errors, fabricated information, unsupported claims, and misleading responses produced by leading AI language models.

## Project Status

This project is currently under development.

The initial goal is to create a small collection of carefully documented hallucination examples and gradually develop a repeatable system for comparing AI model responses.

## Purpose

Large language models can produce answers that sound confident and convincing even when the information is incorrect, unsupported, outdated, or entirely fabricated.

This repository documents those failures in a structured format.

The project is intended to demonstrate practical skills in:

- comparing responses from multiple AI models;
- identifying factual and reasoning errors;
- verifying claims using reliable evidence;
- distinguishing minor mistakes from serious failures;
- documenting model behavior consistently;
- building structured datasets for later analysis.

## Models Evaluated

The project may include responses from:

- OpenAI GPT models
- Anthropic Claude models
- Google Gemini models
- other language models when relevant

The model name, version, and test date will be recorded whenever that information is available.

## What Each Evaluation Contains

Each completed evaluation will include:

1. The original prompt
2. The GPT response
3. The Claude response
4. The Gemini response
5. The hallucination or error identified
6. The correct information
7. Supporting evidence and sources
8. An explanation of the correction
9. A severity rating
10. Evaluator notes
11. The date tested
12. The model version, when available

## Hallucination Categories

Examples may include:

- fabricated facts;
- fabricated citations or sources;
- incorrect dates;
- incorrect names or attributions;
- false quotations;
- unsupported numerical claims;
- outdated information presented as current;
- conflation of separate people or events;
- contradictions within a response;
- overconfident answers without sufficient evidence;
- incorrect legal, medical, financial, scientific, or historical claims.

## Severity Scale

| Severity | Description |
|---|---|
| Low | A minor error that does not substantially change the answer |
| Medium | A meaningful factual error or misleading omission |
| High | A major error that changes the conclusion or seriously misleads the user |
| Critical | An error that could contribute to legal, medical, financial, physical, or other serious harm |

## Evaluation Principles

Evaluations should be:

- evidence-based;
- reproducible when possible;
- clearly documented;
- fair to each model;
- based on the same prompt and comparable testing conditions;
- explicit about uncertainty;
- updated when stronger evidence becomes available.

A disagreement with a model is not automatically a hallucination. Each identified error should be supported by reliable evidence.

## Planned Repository Structure

```text
AI-Hallucination-Database/
│
├── README.md
├── CONTRIBUTING.md
├── LICENSE
│
├── schema/
│   ├── evaluation-schema.md
│   └── evaluation-template.yaml
│
├── evaluations/
│   ├── history/
│   ├── science/
│   ├── law/
│   ├── medicine/
│   ├── geography/
│   ├── technology/
│   └── current-events/
│
├── datasets/
│   ├── hallucinations.csv
│   └── hallucinations.json
│
├── evidence/
│   └── archived-sources/
│
└── scripts/
    ├── validate_entries.py
    └── build_dataset.py
