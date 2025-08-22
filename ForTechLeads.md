# AI Security Guidelines for Tech Leads, Heads, and Architects

## Oversight & Policy

- **Mandate remote repositories** (Bitbucket, GitHub, etc.) for all AI-assisted projects.  
  Local-only repos are not permitted for AI code development.

- **Enforce repo tagging:**  
  Require a `.ai-used` file at the root of every repo where AI tools (LLMs, code assistants) are used.



<pre>
# .ai-used
AI tools (LLMs, code assistants) were used to write code in this repository.
</pre>

#### Sample File
See the [`.ai-used`](ai-used.md) file for compliance details.

This tag enables the security team to apply **mandatory scans, tracking, and audit checks**.



## Review & Compliance

- **Ensure all AI-assisted repos undergo:**
  - **SAT** (Static Application Testing)
  - **SCA** (Software Composition Analysis)
  - **Secret scanning** (prioritized)

- **Monitor for compliance:**  
  Regularly audit repos for `.ai-used` tagging and security scan results.

## Secure Development Practices

- **Promote minimal, relevant code sharing with AI tools.**
- **Prohibit sharing of secrets, credentials, or sensitive data with AI.**
- **Encourage use of only approved tools and endpoints.**
- **Require credential rotation if exposure is suspected.**

## Support & Escalation

- **Contact the security team:**  
  For help with secure local environment setup or policy questions, email [whitehat@timesinternet.in](mailto:whitehat@timesinternet.in).

- **Escalate any suspected data exposure or security incident immediately.**

## ⚠️ Leadership Responsibility

Tech Leads, Heads, and Architects must ensure that:  
- AI-assisted development aligns with **org-wide security policies**.  
- Repos are properly **tagged, scanned, and monitored**.  
- Teams understand and adhere to the **Do’s & Don’ts of AI tool usage**.  

Failure to enforce these practices may result in **security risks, compliance breaches, and accountability actions**.