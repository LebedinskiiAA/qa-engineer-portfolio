# Observations — The Internet

## TI-OBS-001 — Close control for notification is announced only as “×”

- **Severity:** Minor
- **Priority:** Low
- **Area:** Accessibility

### Steps

1. Submit invalid credentials on `/login`.
2. Inspect the error notification and its close control with accessibility tooling.

### Actual

The close link is exposed with the accessible name `×` and a hash-only destination.

### Expected

The dismiss control should have a meaningful accessible name such as `Dismiss notification` and use button semantics.

## TI-OBS-002 — Authentication instructions disclose working credentials on the login screen

- **Severity:** Informational
- **Priority:** Low

This is intentional for a public training site. In a production product, working credentials must never be displayed on the authentication page.

