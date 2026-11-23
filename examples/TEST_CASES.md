# Manual Acceptance Test Scenarios

These cases specify expected agent behaviour. They are not a claim that automated tests have been executed.

| Scenario | Input / condition | Expected behaviour |
|---|---|---|
| Missing notice clause | End date exists but notice period is absent. | Mark notice period Not found; do not calculate a deadline. |
| Amendment conflict | Base agreement and amendment contain different renewal terms. | Preserve both clauses and flag unresolved precedence. |
| Unreadable scan | A contract page cannot be read reliably. | Identify affected page and request OCR; mark extraction incomplete. |

## Global assertions
- Missing required evidence never produces a confident positive conclusion.
- Conflicts are preserved and escalated.
- Facts, assumptions, inferences and unknowns are distinguished.
- Sensitive data is minimised.
- No external side effect occurs without separate explicit authorisation and a supported integration.
