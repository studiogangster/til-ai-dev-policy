# Best Practices for AI-Assisted Code Development

## 1. Always Use a Remote Repository

- Create a remote repository (Bitbucket, GitHub, etc.) for every new project using AI code editors.
- Avoid working only in local repositories to ensure auditability and backup.

## 2. Tag AI Usage in the Repo

- Add a file named `.ai-used` at the root of your repository to indicate AI tools were used.

<pre>
# .ai-used
AI tools (LLMs, code assistants) were used to write code in this repository.
</pre>

## 3. Secure Coding with AI Editors

- Share only minimal, relevant code snippets with AI tools.
- Never share secrets, credentials, or sensitive data.
- Redact or mask any sensitive information before using AI suggestions.
- Use only approved endpoints and tools.
- Rotate credentials immediately if pasted or exposed.
- Do not paste or share:
  - `.env` files
  - Private keys
  - Customer data
  - Entire repositories
  - Production configs

## 4. Security Scanning & Compliance

- All AI-assisted repos **must** go through:
  - **SAT** (Static Application Testing)
  - **SCA** (Software Composition Analysis)
  - **Secret scanning** (on priority)


## 5. Contact Security Team

- For help with secure local environment setup or policy questions, email [whitehat@timesinternet.in](mailto:whitehat@timesinternet.in).
