# Multilingual Localization & Linguistic QA Toolkit

A practical, language-agnostic toolkit for planning, reviewing and improving multilingual content. It is designed for localization project managers, translators, editors, reviewers and AI language-evaluation teams.

The toolkit turns quality expectations into repeatable workflows: define the brief, manage terminology, review meaning and language, classify defects, calibrate reviewers, and document decisions.

## Scope

Use this toolkit for translation, localization, subtitling, multilingual editorial work, linguistic data and AI-generated language outputs. Adapt the checks to the content type, locale, audience, risk level and client requirements.

It is a general-purpose, independently developed resource. It does not reproduce confidential client procedures or claim certification against a particular industry standard.

## Toolkit contents

- [Error taxonomy](ERROR_TAXONOMY.md): defect categories, severity and correction principles.
- [Terminology workflow](TERMINOLOGY_WORKFLOW.md): term research, approval, implementation and maintenance.
- [Reviewer calibration](REVIEWER_CALIBRATION.md): onboarding, sample review, adjudication and consistency.
- [QA checklist](QA_CHECKLIST.md): practical checks before delivery.
- [Synthetic example](examples/pt-en-review-example.md): an illustrative review with issue classification and rationale.

## Recommended workflow

1. **Understand the assignment.** Confirm source and target locales, audience, purpose, content type, reference materials, formatting, platform constraints and delivery criteria.
2. **Establish linguistic controls.** Identify approved terminology, style rules, locale conventions and authoritative references.
3. **Translate or generate.** Work from the approved brief and preserve meaning, intent, register and required structure.
4. **Review against the source.** Check completeness, accuracy, terminology, grammar, style, locale and functional constraints.
5. **Classify and correct defects.** Record the issue, evidence, severity, proposed correction and rationale.
6. **Run final QA.** Verify corrections, consistency, formatting and delivery requirements.
7. **Learn from results.** Track recurring patterns and update guidance, glossaries and calibration examples.

## Quality principles

- Meaning takes priority over word-for-word similarity.
- A fluent sentence can still be inaccurate or incomplete.
- Do not infer facts, intent or context that the source does not support.
- Distinguish objective errors from defensible stylistic preferences.
- Apply locale conventions consistently.
- Record uncertainty and escalate material ambiguity rather than silently guessing.
- Evaluate impact in context: a minor punctuation issue and a reversed medical instruction are not equivalent.
- Keep an audit trail for consequential decisions.

## Suggested issue record

For each defect, record:

| Field | What to capture |
|---|---|
| ID | Unique issue identifier |
| Location | Segment, timestamp, page or UI string |
| Source | Relevant source text or reference |
| Target | Current target text |
| Category | Taxonomy category |
| Severity | Critical, major, minor or preference |
| Rationale | Why the target is defective, with evidence |
| Correction | Proposed target or action |
| Status | Open, corrected, accepted or escalated |
| Reviewer | Reviewer or adjudicator |

## Adaptation and limitations

This toolkit is a starting point, not a substitute for domain-specific review, legal or regulatory requirements, accessibility testing, functional testing or client-approved specifications. For high-risk content—such as medical, legal, financial or safety-critical material—use qualified subject-matter review and the applicable governance process.

All examples in this repository are synthetic and are provided for demonstration and training.
