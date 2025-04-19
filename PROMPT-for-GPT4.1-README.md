Below is a **universal prompt template for GPT‑4.1** plus guidance on how to adapt it.
Feel free to copy‑paste and swap the bracketed placeholders. citeturn0search0

---

```markdown
# 💼 Role & Objective
You are **{role}**.
Your goal is **{objective}**.

# 📜 High‑Level Instructions
- {rule 1}
- {rule 2}
- {rule 3}

## 🔧 Tool Usage  *(include only if the model can call tools)*
- Persist until the task is completely solved; **do not** yield control early.
- If unsure, call available tools to inspect data—**never** guess.
- *(Optional)* Before each tool call, write a short plan; after the call, reflect on the result.

# 🧩 Reasoning Steps  *(for chain‑of‑thought)*
1. Analyse the user’s request and clarify intent.
2. Retrieve or reference relevant context.
3. Think **step by step** to draft the answer or decide the next action.
4. Verify the answer against requirements and edge cases.

# 🖨️ Output Format
Respond in **{format}**.
- Add citations like `[TITLE](ID)` immediately after any factual claim.
- Use emojis 🎯 sparingly / never (choose one).

# 📝 Examples
## Example 1
**User**: {sample_user_input}
**Assistant**: {sample_assistant_output}

---

# 🚀 Final Instruction
Follow **all** rules above.
If information is missing, **ask the user**; do *not* hallucinate.
Begin now ↓
```

---

### How each section works

| Section | Purpose | Tips |
|---------|---------|------|
| **Role & Objective** | Tell the model what persona to adopt and the final goal in one line. | e.g. *You are a financial‑risk analyst…* |
| **High‑Level Instructions** | Non‑negotiable rules: tone, limits, taboo topics. | List by priority; avoid vague words. |
| **Tool Usage** | Embeds the Persistence / Tool‑calling / (optional) Planning triad that boosts GPT‑4.1 agent performance. | Keep it to 2‑3 bullet points—long lists dilute impact. |
| **Reasoning Steps** | Induces visible chain‑of‑thought without over‑prompting. | 3–5 lines are enough; refine after observing failures. |
| **Output Format** | Guarantees machine‑readable answers. | Add a short example if breaking the format is fatal. |
| **Examples** | One or two successes illustrating every rule. | Wrap more examples in `<example>` tags or Markdown sub‑sections if needed. |
| **Final Instruction** | Last word wins if rules conflict. | GPT‑4.1 tends to obey the last instruction most strongly. |

---

### Quick variants

| Scenario | What to tweak |
|----------|---------------|
| **Coding‑fix agent** | Keep Tool Usage mandatory; expand Reasoning Steps to *Plan → Call python → Reflect → Test*. |
| **Long‑document QA** | Duplicate key instructions both *above* and *below* the huge context; add “Use only external context unless specified”. |
| **One‑off Q&A** | Remove Tool Usage and Reasoning Steps; keep concise High‑Level rules. |

---

### Best‑practice checklist

1. **Be explicit and positive.** “Only call a tool if sure” is clearer than “don’t call tools unnecessarily.”
2. **One‑sentence nudges work.** If behaviour drifts, add or edit a single line at the top or bottom.
3. **Iterate fast with evals.** GPT‑4.1 may evolve; keep an end‑to‑end test suite in CI to catch regressions.

Use this skeleton as your starting point, prune or expand each block, and evolve it alongside your real‑world tests.
