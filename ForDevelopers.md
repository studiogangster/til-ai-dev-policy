# 🔒 AI Security Guidelines for Developers

## 🚀 Getting Started

- **Always create a remote repository** (Bitbucket, GitHub, etc.) for any new project using AI code editors.  
  ❌ Do **not** work only in a local repo.  
- **Use private repositories under the official org account only.**  
  Personal accounts or public repos are not allowed.  

- **Tag your repo for transparency:**  
  Add a `.ai-used` file at the root of your repository.  

# .ai-used
<pre>
AI tools (LLMs, code assistants) were used to write code in this repository.
</pre>

## 🔒 AI Usage Declaration

This project uses AI-assisted code development.  
See the [`.ai-used`](ai-used.md) file for compliance details.

---

## 🧑‍💻 Coding Practices with AI Code Editors

- ✅ Share only **minimal, relevant snippets** (not full files or repos).  
- ✅ Redact or mask sensitive info **before** sending to AI tools.  
- ✅ Use only **approved endpoints and editors**.  
- ✅ Rotate credentials immediately if **pasted or exposed**.  

- 🚫 Do **not** paste or share:
  - `.env` files  
  - 🔑 Private keys or tokens  
  - 👤 Customer data (PII/PHI/PCI)  
  - 📦 Entire repositories  
  - ⚙️ Production configs  

---

## 🛡️ Security Requirements (Mandatory)

All AI-assisted repositories **must undergo** the following before deployment:  

- 🔍 **SAT** – Static Application Testing  
- 📦 **SCA** – Software Composition Analysis  
- 🕵️ **Secret Scanning** – High priority  

⚠️ No **Critical** or **High** vulnerabilities may remain before release.  

---

## 📬 Need Help?

If you need assistance setting up a secure environment or have any concerns:  

**✉️ [whitehat@timesinternet.in](mailto:whitehat@timesinternet.in)**  

---

> ⚠️ **Reminder:**  
> AI tools are **accelerators**, not replacements for **secure coding, peer review, and compliance checks**.  
> Every AI-generated output must be validated.
