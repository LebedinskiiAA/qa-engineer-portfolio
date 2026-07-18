# Defect Reports — SauceDemo

## SD-BUG-001 — All inventory items use the same fallback image for `problem_user`

- **Severity:** Major
- **Priority:** High
- **Environment:** Desktop browser, https://www.saucedemo.com/, 18 July 2026
- **Precondition:** Public `problem_user` test account is available.

### Steps to reproduce

1. Open the login page.
2. Sign in as `problem_user` with the published test password.
3. Review all six inventory cards.

### Actual result

All six products reference the same `/assets/sl-404-...jpg` image although their names and descriptions are different.

### Expected result

Each inventory card displays the image corresponding to its product.

### Impact

Customers cannot visually distinguish products; the catalog appears unreliable.

## SD-BUG-002 — Product and menu navigation links expose `href="#"`

- **Severity:** Minor
- **Priority:** Medium
- **Type:** Accessibility / navigation observation

### Actual result

Product title/image links and several menu links expose a hash-only destination and depend entirely on client-side handlers.

### Expected result

Interactive links should expose stable, meaningful destinations so they remain understandable to assistive technology and support standard browser actions such as copying a link.

### Note

This is a semantic/accessibility observation. Functional navigation should be verified separately with keyboard and assistive-technology testing.

