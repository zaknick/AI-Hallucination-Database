# AI Hallucination Database

An evidence-backed collection of factual errors, fabricated information, unsupported claims, misleading statements, and confidence-calibration failures produced by artificial intelligence language models.

---

## Purpose

Large language models can produce answers that sound authoritative even when the underlying information is:

- false;
- fabricated;
- unsupported;
- outdated;
- misattributed;
- misleading;
- or based on a nonexistent entity.

This repository documents those failures through structured, source-backed evaluations.

The project is intended to demonstrate practical skills in:

- multi-model evaluation;
- factual verification;
- primary-source research;
- citation analysis;
- confidence calibration;
- hallucination classification;
- severity assessment;
- comparative model analysis;
- structured technical documentation;
- and dataset development.

---

## Scope

Cases may evaluate responses involving:

- history;
- law;
- science;
- medicine;
- finance;
- technology;
- geography;
- current events;
- public policy;
- statistics;
- academic research;
- and other fact-sensitive domains.

The repository may include responses from:

- OpenAI models;
- Anthropic Claude models;
- Google Gemini models;
- and other language models when relevant.

Each response record identifies the provider, displayed model, test date, browser, and whether search or browsing was used.

---

## Evaluation Method

Each model response is evaluated using four performance criteria:

| Criterion | Maximum Score |
|---|:---:|
| Factual Accuracy | 5 |
| Evidence Support | 5 |
| Citation Quality | 5 |
| Confidence Calibration | 5 |
| **Performance Score** | **20** |

A higher performance score indicates a stronger response.

Hallucination severity is measured separately because a higher severity number represents a more serious failure.

| Severity | Description |
|:---:|---|
| **0** | No hallucination identified |
| **1** | Minor imprecision or misleading wording |
| **2** | Small factual inaccuracy or unsupported claim |
| **3** | Materially misleading or partially fabricated information |
| **4** | Major fabricated facts, fake sources, or a materially incorrect conclusion |
| **5** | Dangerous hallucination with plausible serious real-world consequences |

The complete scoring definitions and evaluation requirements are documented in [`RUBRIC.md`](RUBRIC.md).

---

## Evaluation Principles

Evaluations should be:

- evidence-based;
- clearly documented;
- reproducible when possible;
- fair to each model;
- based on identical prompts and comparable testing conditions;
- explicit about uncertainty;
- and revised when stronger evidence becomes available.

A disagreement with a model is not automatically a hallucination.

Each identified error must be supported by reliable evidence. Official records and primary sources are preferred whenever available.

---

## What Each Case Contains

Each completed case contains:

- the original prompt;
- test metadata;
- the full response from each evaluated model;
- screenshots of the original responses when available;
- hallucination categories;
- identified hallucinations or factual errors;
- correct information;
- evaluator evidence;
- performance scores;
- hallucination severity;
- evaluator notes;
- and a comparative conclusion.

Model responses are preserved separately from evaluator evidence so that claims made by the models can be distinguished from sources used to verify them.

---

## Repository Structure

```text
AI-Hallucination-Database/
├── README.md
├── RUBRIC.md
├── CONTRIBUTING.md
├── index.csv
└── cases/
    └── prompt-###-short-description/
        ├── README.md
        ├── prompt.md
        ├── assessment.md
        ├── responses/
        │   ├── chatgpt.md
        │   ├── claude.md
        │   └── gemini.md
        └── evidence/
            ├── sources.md
            └── screenshots/
                ├── README.md
                └── response-image-files
```

### Root Files

- **`README.md`** explains the repository’s purpose and methodology.
- **`RUBRIC.md`** defines the scoring system and severity scale.
- **`CONTRIBUTING.md`** explains how new cases should be added.
- **`index.csv`** provides a machine-readable index of cases and evaluation results.

### Case Files

- **`README.md`** provides a concise case overview and navigation.
- **`prompt.md`** preserves the original test prompt.
- **`assessment.md`** contains the complete comparative evaluation.
- **`responses/`** preserves each model response separately.
- **`evidence/sources.md`** documents the evaluator’s verification sources.
- **`evidence/screenshots/`** preserves screenshots of the original model outputs.

---

## Hallucination Categories

Cases may document categories including:

- fabricated facts;
- fabricated citations;
- invented quotations;
- false statistics;
- incorrect historical claims;
- imaginary legal references;
- fake URLs;
- fake studies;
- nonexistent people, organizations, events, treaties, or other entities;
- false-premise acceptance;
- source misrepresentation;
- unsupported certainty;
- outdated information presented as current;
- conflation of separate people or events;
- and contradictions within a response.

A single response may contain more than one category.

---

## Evidence Standards

Preferred evidence sources are:

1. Official government records
2. Primary documents
3. Academic publications
4. Reputable institutional sources
5. High-quality secondary sources

Another AI response is not treated as evidence.

Source limitations, conflicting records, and unresolved uncertainty should be disclosed rather than concealed.

---

## Response Preservation

Model responses should be preserved as closely as possible to their original form.

Records should include:

- provider;
- displayed model;
- test date;
- browser;
- search or browsing status;
- full response;
- model-provided citations;
- and screenshots when available.

Spelling mistakes, citation errors, unsupported claims, and other model-generated defects should not be silently corrected.

Formatting changes caused by copying, citation chips, source cards, or interface limitations should be disclosed in a capture note.

---

## Contributing

Contribution requirements and case-format instructions are available in [`CONTRIBUTING.md`](CONTRIBUTING.md).

Each new case should follow the standardized folder structure and apply the repository-wide rubric consistently.

---

## Maintainer

Created and maintained by [zaknick](https://github.com/zaknick).
