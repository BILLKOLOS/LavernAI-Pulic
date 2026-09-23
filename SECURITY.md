# Security Policy

At LavernAI, we take the security of our users and their data very seriously. We actively invite security researchers, pentesters, and ethical hackers to responsibly disclose any vulnerabilities found within the LavernAI ecosystem.

## Supported Versions

Only the most recent production versions of the LavernAI APK and live platform are currently in scope for security reports.

## In Scope

The following components are in scope for responsible security testing:
* **LavernAI APK** (Latest production release)
* **Public API Endpoints** (e.g., `api.lavernai.com` - *placeholder*)
* **Web Application** (e.g., `app.lavernai.com` - *placeholder*)

## Out of Scope (Strictly Prohibited)

The following activities and targets are strictly out of scope and explicitly prohibited. Engaging in these activities may result in legal action:
* **Live Gem Wallets & Redemptions:** Do NOT attempt to manipulate Gem balances (purchased, earned, or redeemable buckets), simulate fake match wins to farm Gems, or test vulnerabilities against any live payment or redemption gateways.
* **Live User Data:** Do NOT access, modify, or interact with other users' accounts, wallets, ELO ratings, or private data. Test only on accounts you own and control.
* **Denial of Service (DoS/DDoS):** Do NOT conduct any testing that impairs the availability of LavernAI services or background engines (e.g., the Ladder Competition engine).
* **Social Engineering / Phishing:** Do NOT target LavernAI employees, partners, or users.
* **Physical Security:** Do NOT attempt physical attacks against LavernAI offices or data centers.

## How to Report a Vulnerability

Please do not open a public issue for security vulnerabilities. Instead, report them privately using one of the following methods:

1. **GitHub Security Advisory:** Submit a private vulnerability report via the [Security Advisory tab](#) (if enabled on this repository).
2. **Email:** Send your report directly to our security team at `security@lavernai.com` (placeholder).

Please provide as much information as possible, including:
* A detailed description of the vulnerability.
* Clear, step-by-step instructions to reproduce the issue.
* The potential impact of the vulnerability.
* Suggested mitigation or fix (if known).

*You may use our `.github/ISSUE_TEMPLATE/pentest_finding.md` format for structuring your report via email.*

## Response Time Commitment

We are committed to addressing security reports promptly:
* **Acknowledgment:** We will acknowledge receipt of your report within **3 business days**.
* **Triage/Assessment:** We aim to triage and confirm the vulnerability within **7 business days**.
* **Resolution:** Time to fix depends on severity, but we prioritize critical and high-severity issues immediately.

## Hall of Fame

We deeply appreciate the efforts of the security community. Researchers who responsibly disclose valid, previously unknown vulnerabilities that result in a code or configuration change will be recognized in our Security Hall of Fame (with their permission).
