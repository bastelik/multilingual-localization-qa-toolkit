# Synthetic Review Example: Portuguese to English

This example demonstrates how to document a linguistic issue without relying on reviewer preference. The scenario and text are fictional.

## Brief

Translate a short product notice from Brazilian Portuguese into English. Preserve the level of certainty and do not add claims that are absent from the source.

## Source

> O aplicativo pode solicitar uma nova verificação de identidade quando houver alterações nos dados da conta.

## Draft target

> The app will require users to verify their identity again whenever their account details change.

## Review findings

### Issue 1 — Modality and certainty

- **Category:** Accuracy — distortion
- **Severity:** Major (illustrative; final severity depends on product context)
- **Evidence:** “pode solicitar” expresses possibility and “when there are changes” does not necessarily mean every change triggers the event.
- **Finding:** “will require” turns a possibility into certainty. “Whenever” may also imply that every change triggers a verification.
- **Suggested correction:** “The app may request a new identity verification if the account details change.”

### Issue 2 — Actor and action

- **Category:** Accuracy — distortion / terminology, depending on product terminology
- **Severity:** Minor to major, depending on whether “request” and “require” have distinct product meanings.
- **Evidence:** The source says the app may request a verification, not necessarily require the user to complete one.
- **Finding:** “Require users” may imply an obligation stronger than the source.
- **Suggested correction:** Retain “may request” unless product documentation establishes a stronger requirement.

## Revised target

> The app may request a new identity verification if the account details change.

## Reviewer rationale

The revision preserves the source's uncertainty and avoids making the trigger sound automatic. It does not add a claim about what happens if the user does not complete verification.

## Calibration questions

1. Which words in the source establish uncertainty?
2. Does “whenever” preserve the source's conditional meaning?
3. What product reference would help determine whether “request” or “require” is the approved term?
4. Would the severity change if the notice concerned access to a regulated financial service?

## Learning point

A target sentence can be grammatically correct and fluent while materially changing the source. Reviewers should compare claims, conditions and degrees of certainty—not just readability.
