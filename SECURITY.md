# Security Policy

At LavernAI, we take the security of our platform — and the safety of every student, teacher, and community member who uses it — extremely seriously. LavernAI handles sensitive educational data, Gem wallet balances, and integrates with real payment providers (Paystack / M-PESA). Protecting that ecosystem is a top priority.

We actively invite security researchers, pentesters, and ethical hackers to responsibly disclose any vulnerabilities found within the LavernAI ecosystem. If you find something, we want to hear about it — and we'll credit you for it.

---

## Supported Versions

| Component | Supported Version |
|---|---|
| LavernAI Android APK | Latest production release on [GitHub Releases](https://github.com/BILLKOLOS/LavernaiClientBetatest/releases) |
| LavernAI Web App | Current live deployment |
| LavernAI Public API | Current live endpoints |

Only the **most recent production versions** are in scope. Vulnerabilities in deprecated or beta builds will be evaluated on a case-by-case basis.

---

## In Scope

The following components are fair game for responsible security testing:

| Target | Description |
|---|---|
| **LavernAI APK** | The Android application — reverse engineering, local storage inspection, intent hijacking, insecure data leakage, etc. |
| **Public API Endpoints** | REST API endpoints serving the mobile and web clients — authentication bypass, IDOR, injection, broken access control, etc. |
| **Web Application** | The browser-based LavernAI platform — XSS, CSRF, session management, open redirects, etc. |
| **Authentication & Session Management** | Token handling, session expiry, password reset flows, OAuth flows |
| **Gem Economy Logic** | Flaws in the Gem earning, spending, or redemption logic that could allow illegitimate Gem generation or unauthorized cashout |
| **Competition Integrity** | Exploits that could manipulate ELO rankings, competition results, question answers, or room state |
| **Socket.IO / Real-time Layer** | Unauthorized event emission, lobby manipulation, race conditions in live play |

---

## Out of Scope (Strictly Prohibited)

The following activities and targets are **strictly out of scope** and explicitly prohibited. Engaging in these activities may result in legal action:

* **Real Financial Transactions:** Do NOT test vulnerabilities against live Paystack or M-PESA payment gateways. Do NOT attempt to trigger real money transfers, initiate fraudulent payouts, or manipulate live wallet balances.
* **Live Gem Wallet Manipulation:** Do NOT attempt to manipulate Gem balances (purchased, earned, or redeemable buckets) on accounts you do not own. Do NOT attempt to exploit the redemption system to extract real KES.
* **Other Users' Data:** Do NOT access, modify, exfiltrate, or interact with other users' accounts, personal data, wallets, ELO ratings, or competition history. Test **only on accounts you own and control**.
* **Denial of Service (DoS/DDoS):** Do NOT conduct any testing that degrades or impairs the availability of LavernAI services, including the autonomous Ladder Competition engine, Socket.IO servers, or database infrastructure.
* **Social Engineering / Phishing:** Do NOT target LavernAI employees, educators, students, partners, or users with social engineering, phishing, vishing, or pretexting attacks.
* **Physical Security:** Do NOT attempt physical attacks against LavernAI offices, personnel, or hosting infrastructure.
* **Automated Scanners at Scale:** Do NOT run aggressive automated vulnerability scanners (e.g., mass fuzzing, brute-force) against production systems without prior written approval.
* **Third-Party Services:** Vulnerabilities in services we depend on (e.g., Paystack, Firebase, MongoDB Atlas, Render) should be reported directly to those providers, not to us.

---

## How to Report a Vulnerability

**⚠️ Please do NOT open a public GitHub issue for security vulnerabilities.** Public disclosure puts our users at risk.

Instead, report privately using one of these methods:

### Option 1: GitHub Security Advisory (Preferred)
Submit a private vulnerability report directly through GitHub's built-in Security Advisory system:

👉 **[Report a Vulnerability via GitHub Security Advisory](https://github.com/BILLKOLOS/LavernAI-Pulic/security/advisories/new)**

This is the fastest and most secure method. Your report stays private and only the repository maintainers can see it.

### Option 2: Email
Send your report directly to our security lead:

📧 **billooko2@gmail.com**

Subject line: `[SECURITY] Brief description of the vulnerability`

### What to Include in Your Report

Please provide as much detail as possible:
* **Vulnerability Title** — A short, descriptive name
* **Severity Assessment** — Critical / High / Medium / Low
* **Affected Component** — APK, API endpoint, Web App, Gem Economy, Competition system, etc.
* **Detailed Description** — What the vulnerability is and how it works
* **Step-by-Step Reproduction** — Clear instructions so we can reproduce and verify
* **Proof of Concept** — HTTP requests, screenshots, video recordings, code snippets
* **Impact Assessment** — What could an attacker achieve? (e.g., unauthorized data access, account takeover, Gem inflation)
* **Suggested Fix** — If you have a recommendation, we'd love to hear it

*You may also use our [Pentest Finding Template](https://github.com/BILLKOLOS/LavernAI-Pulic/blob/main/.github/ISSUE_TEMPLATE/pentest_finding.md) to structure your report.*

---

## Response Time Commitment

We are committed to addressing security reports promptly:

| Stage | Timeframe |
|---|---|
| **Acknowledgment** | Within **48 hours** of receipt |
| **Triage & Validation** | Within **7 business days** |
| **Status Update** | You will receive regular updates until the issue is resolved |
| **Critical/High Severity Fix** | Prioritized immediately; target resolution within **14 days** |
| **Medium/Low Severity Fix** | Addressed in the next scheduled release cycle |

If you don't hear back within 48 hours, please follow up — emails can get lost and we genuinely want to respond.

---

## Safe Harbor

LavernAI supports responsible security research. If you conduct your research in accordance with this policy, we will:

* **Not pursue legal action** against you for your research activities
* **Not report your testing** to law enforcement, provided you follow this policy
* **Work with you** to understand and resolve the issue quickly
* **Recognize your contribution** publicly (with your permission)

We ask that you:
* Act in good faith and avoid privacy violations, data destruction, or service disruption
* Only interact with accounts you own or have explicit permission to test
* Stop testing and report immediately if you encounter any user data
* Give us a reasonable window to fix the issue before any public disclosure (minimum 90 days)

---

## Hall of Fame 🏆

We deeply appreciate the security community. Researchers who responsibly disclose valid, previously unknown vulnerabilities that result in a code or configuration change will be recognized here (with their permission).

| Researcher | Finding | Date |
|---|---|---|
| *Your name could be here!* | — | — |

Want to be listed? Include your preferred name/handle, X/Twitter, or LinkedIn in your report and let us know you'd like credit.

---

## Questions?

If you have questions about this policy or want to discuss scope before testing, reach out to **billooko2@gmail.com** — we're happy to clarify.
