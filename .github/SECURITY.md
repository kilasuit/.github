# Security Policy

## Reporting a vulnerability

**Please do not report security vulnerabilities in public GitHub issues.**

### Preferred method: GitHub Private Vulnerability Reporting

Use GitHub's built-in [Private Vulnerability
Reporting][private-vulnerability-reporting] on the affected repository:

1. Navigate to the repository on GitHub.
2. Click **Security** → **Advisories** → **Report a vulnerability**.
3. Fill in the form with as much detail as you can provide.

This creates an encrypted draft security advisory visible only to maintainers
and the Org Admin.

### Fallback method: email

If GitHub Private Vulnerability Reporting is unavailable or you prefer email:

**<security@kilasuit.org>**

### What to include

A useful report includes:

- A description of the vulnerability and the potential impact
- The affected repository
- Steps to reproduce or a proof-of-concept
- Any known mitigations or workarounds
- Your preferred contact method for follow-up

If sending by Email this **must** be encrypted and signed using the PGP Key as listed on https://blog.kilasuit.org/contact-me/

---

## Our commitments

Once we receive your report:

| Milestone                                             | Target   |
| ----------------------------------------------------- | -------- |
| Acknowledge receipt & provide a preliminary status    | 84 hours |
| Provide a follow up status update                     | 7 days   |
| Deliver fix or mitigation for **critical** severity   | 14 days  |
| Deliver fix or mitigation for **high** severity       | 30 days  |
| Deliver fix or mitigation for **medium/low** severity | 90 days  |

These are targets, not guarantees. If I need more time, I'll will tell you why.

---

## Coordinated disclosure

We follow the widely accepted coordinated disclosure model:

1. Reporter submits the vulnerability privately.
2. Maintainers validate and develop a fix.
3. We agree on an embargo period (typically 14–90 days depending on severity and
   fix complexity).
4. A patched release is published.
5. A GitHub Security Advisory is published, credited to the reporter unless they
   prefer to remain anonymous.
6. For serious vulnerabilities we will request a CVE from a CNA; this typically
   happens at or before public disclosure.

We ask that reporters:

- Allow us the agreed embargo window before public disclosure
- Avoid exploiting the vulnerability beyond what is needed to demonstrate it
- Avoid accessing or modifying data belonging to others

In return, we commit to:

- Keeping you informed throughout the process
- Crediting you in the advisory and release notes (unless you prefer anonymity)
- Acting in good faith to resolve the issue promptly

---

## Out of scope

The following are generally not in scope for security reports:

- Vulnerabilities in libraries or products that we consume - These should be directed to their own programs.
- Issues that require the attacker to already have administrative or write
  access to the affected system
- Denial-of-service attacks that require significant resources from the attacker
- Social engineering of maintainers or contributors

If you are unsure whether your finding is in scope, report it anyway — we would
rather review a borderline finding than miss a real one.

---

## Questions

General security questions (not vulnerability reports) should be asked in issues in their respective repos.
[private-vulnerability-reporting]:
  https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability
