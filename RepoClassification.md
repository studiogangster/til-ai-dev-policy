# 🗂️ Repo Classification

All repositories must be classified into one of the following categories before AI tools are used.

---

## 🟢 Green – Safe for Cloud AI

- ✅ Demo repos, boilerplate, open source examples  
- ✅ No sensitive or proprietary data  
- ✅ Approved for **cloud-based AI tools** (OpenAI, Anthropic, Azure OpenAI, etc.)  
- ⚠️ Still must follow standard secure coding practices  

**Tag:** `AI:Green`

---

## 🟡 Yellow – Limited AI (Guardrails Required)

- ⚠️ Contains internal business logic or infrastructure templates  
- ⚠️ May include sensitive configurations  
- ⚠️ AI usage allowed but only with **strict guardrails + peer review**  
- ⚠️ Requires Tech Lead approval before AI code is committed  

**Tag:** `AI:Yellow`

---

## 🔴 Red – No Cloud AI (Local/Offline Only)

- 🚫 Cryptography libraries or implementations  
- 🚫 Customer data, regulated data (PII, PHI, PCI)  
- 🚫 Security tools or sensitive internal frameworks  
- 🚫 **Cloud AI tools are forbidden** – use only approved local/offline models  

**Tag:** `AI:Red`

---

## 🔍 Classification Ownership

- **Tech Teams** → apply initial classification and add `.ai-used` if AI tools are used.  
- **Security Team** → validates classifications, and may **adjust/override** based on risk.  
- **Future updates** → new tags or classification changes will be communicated to each business unit individually.  

---

## 📝 Repo Tagging

Every AI-assisted repo must contain a `.ai-used` file:

<pre>
# .ai-used
AI tools (LLMs, code assistants) were used to write code in this repository.
</pre>

---


