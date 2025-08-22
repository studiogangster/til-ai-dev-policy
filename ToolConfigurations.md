# IDE & Extension Settings


### **Document Purpose:**  
 Defines **secure defaults, ignore rules, and usage policies** for AI-powered IDEs, extensions, and developer assistants. 
 This ensures **data protection, compliance, and consistent security posture** across teams.


Configure the following settings for your code editors and AI extensions as outlined below; if you face any issues applying them, please contact the Security Team at [whitehat@timesinternet.in](mailto:whitehat@timesinternet.in).

> **Nudge:**  
> If you are using any editor, extension, or AI service not covered in this document, please contact the Security Team at [whitehat@timesinternet.in](mailto:whitehat@timesinternet.in).  
> We will review, provide secure configuration guidance, and update this document to include the missing tool.



---

## VS Code / GitHub Copilot

**Settings Example**
```json
{
  "telemetry.enableTelemetry": false,
  "github.copilot.enable": true,
  "github.copilot.advanced": {
    "context": "manual"
  }
}
```

**.cursorignore Sample**
```
.env
*.key
*.pem
secrets/*
```

---

## VS Code Cline Extension

Cline is an AI-powered code completion and assistant extension for VS Code. To use Cline securely:

**Recommended Settings**
```json
{
  "cline.telemetry": false,
  "cline.contextSharing": "manual",
  "cline.snippetSelection": "manual"
}
```

**Best Practices**
- Disable telemetry to prevent sharing usage data externally.
- Set context sharing to "manual" to avoid automatic sharing of entire files or sensitive code.
- Always select code snippets manually before sending to Cline.
- Never share secrets, credentials, or sensitive data with the extension.
- Use `.clineignore` to exclude files containing secrets or sensitive information.

**.clineignore Sample**
```
.env
*.key
*.pem
secrets/*
```

---

## VS Code CLI (code command)

VS Code provides a command-line interface (`code`) for opening files, folders, and managing extensions directly from the terminal.

**Common Usage:**
```sh
# Open current directory in VS Code
code .

# Open a specific file
code README.md

# Install an extension
code --install-extension ms-python.python

# List installed extensions
code --list-extensions
```

**Best Practices with AI Code Editors:**
- Use the CLI to quickly open remote repositories and ensure you are working in a secure, version-controlled environment.
- Manage extensions via CLI to ensure only approved tools are installed.
- Use CLI commands to automate security scanning and code audits as part of your workflow.

---

## JetBrains AI

**Settings Example**
```json
{
  "ai.telemetry": false,
  "ai.contextSharing": "manual"
}
```

---

## Cursor

**Settings Example**
```json
{
  "cursor.telemetry": false,
  "cursor.contextSharing": "manual"
}
```

**.cursorignore Sample**
```
.env
*.key
*.pem
secrets/*
```

---

## Windsurf

**Settings Example**
```json
{
  "windsurf.telemetry": false,
  "windsurf.contextSharing": "manual"
}
```

**.windsurfignore Sample**
```
.env
*.key
*.pem
secrets/*
```

---

## Claude Desktop

**Settings Example**
```json
{
  "claude.telemetry": false,
  "claude.contextSharing": "manual"
}
```

---


> ## ⚠️ Important
If you use **custom file names or extensions** to store secrets or sensitive files (e.g., `.keys`, `.myenv`, `tokens/`),  
**you must explicitly add them to the relevant ignore file** (`.clineignore`, `.cursorignore`, `.windsurfignore`, etc.)  
to prevent accidental sharing with AI tools or external services.


**Note:**  
Always force manual snippet selection instead of automatic file sharing to minimize risk of leaking sensitive information.
