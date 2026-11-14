# Linguistic QA Error Taxonomy

Use this taxonomy to describe defects consistently across translation, localization, editing, subtitling and AI language evaluation. Select the most specific category that explains the problem. Add a secondary category when a defect has more than one meaningful effect.

## Categories

| Category | Definition | Typical examples |
|---|---|---|
| Accuracy — mistranslation | Target meaning differs from the source | Wrong actor, action, object, condition or relationship |
| Accuracy — omission | Meaningful source information is missing | Dropped warning, qualifier, sentence or UI instruction |
| Accuracy — addition | Target introduces unsupported information | Added promise, explanation, claim or restriction |
| Accuracy — distortion | Meaning is weakened, exaggerated or otherwise shifted | “May” rendered as “will”; uncertainty removed |
| Terminology | Required or established term is not used consistently or correctly | Wrong product term; inconsistent approved equivalent |
| Grammar & syntax | Target violates grammatical or syntactic conventions | Agreement, tense, word order or sentence construction |
| Spelling & orthography | Incorrect spelling, accents, capitalization or punctuation | Misspelling; incorrect diacritics |
| Style & register | Tone, voice or level of formality conflicts with the brief | Informal language in a formal notice |
| Locale & cultural adaptation | Target conflicts with locale conventions or audience expectations | Date, number, currency or culturally inappropriate reference |
| Readability & fluency | Text is difficult to understand or unnatural | Ambiguous construction; calque that impairs comprehension |
| Consistency | Repeated elements are rendered inconsistently without justification | Same feature name translated in multiple ways |
| Formatting & structure | Required structure or formatting is damaged | Broken placeholders, tags, variables, lists or line breaks |
| Functional / technical | Target may fail in the delivery environment | Truncated string, broken markup, placeholder altered |
| Subtitles / timed text | Captioning or timed-text constraints are not met | Reading-speed, line-break, synchronization or speaker-identification issue |
| Brief / instruction adherence | Output fails an explicit assignment requirement | Wrong variant, forbidden terminology, missed word or character limit |

## Severity

Severity should reflect the likely consequence in context, not merely the category.

- **Critical:** Reverses or materially changes meaning in a way that may cause serious harm, legal or financial exposure, safety risk, or a major failure of the intended task. Examples: negation reversed in a medical instruction; dosage or safety warning materially wrong.
- **Major:** Significantly impairs accuracy, usability or the intended message. Examples: key instruction omitted; important entity or condition mistranslated; required term replaced with a misleading one.
- **Minor:** A localized defect with limited impact on comprehension or usability. Examples: non-critical punctuation, agreement or formatting issue.
- **Preference / optional improvement:** A defensible alternative that is not demonstrably wrong and does not violate the brief. Do not count preferences as objective errors unless the project explicitly requires a particular form.

## Classification rules

1. Identify the specific source-target discrepancy or violated requirement.
2. Cite the relevant evidence: source text, approved glossary, style guide, brief or technical specification.
3. Separate the defect from its impact. The category describes what is wrong; severity describes how much it matters.
4. Avoid double-counting one underlying defect as several errors unless it creates distinct consequences.
5. Do not label a stylistic preference as an accuracy error.
6. When the source is ambiguous, record the ambiguity and seek clarification where it materially affects the target.
7. When multiple interpretations are possible, explain why the selected interpretation is best supported.

## Examples

- Source: “The device may overheat.” Target: “O dispositivo vai superaquecer.”  
  Category: Accuracy — distortion. Severity depends on context; the target changes possibility into certainty.
- Source contains a safety warning that is absent from the target.  
  Category: Accuracy — omission. Severity: potentially critical.
- Approved glossary specifies “painel de controlo”; target uses an unapproved alternative in a controlled interface.  
  Category: Terminology. Severity depends on ambiguity and product impact.
- A variable such as `{user_name}` is altered or removed.  
  Category: Formatting & structure and/or Functional / technical. Severity depends on whether the string still works.

## Reporting consistently

A useful issue report states: **what is wrong, where it occurs, what evidence supports the finding, how serious it is, and what action is recommended.** Avoid comments such as “sounds odd” without a specific explanation.
