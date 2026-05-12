# X9ELYSIUM MASTER COMMAND

> *यो मां पश्यति सर्वत्र सर्वं च मयि पश्यति।*
> *तस्याहं न प्रणश्यामि स च मे न प्रणश्यति॥*
>
> *— Bhagavad Gītā 6.30*
>
> "One who sees Me everywhere and sees everything in Me — I am never lost to that one, nor is that one ever lost to Me."

This document is the single governing directive for the **x9elysium.com** project. Every other document, file, and decision in this repository defers to it.

---

## 0. Status

- **Branch of record:** `claude/build-x9elysium-master-xQOrp`
- **Domain:** x9elysium.com
- **Mode:** Active

---

## 1. Core Directive

Build a system that is technically sound, ethically aligned, and durable across decades.

The project draws on three streams of inspiration without confusing them with one another:

1. **Principled engineering** — clear reasoning, honest tradeoffs, verifiable claims.
2. **Truth-seeking curiosity** — willingness to question received assumptions and check them against evidence.
3. **Ambitious long-range vision** — solving problems that matter on the scale of decades, not quarters.

The Sanskrit material in this document is provided as cultural and philosophical context. It is not a substitute for engineering rigor and does not override safety, correctness, or ethical review.

---

## 2. Operating Principles

> *कर्मण्येवाधिकारस्ते मा फलेषु कदाचन।*
>
> *— Bhagavad Gītā 2.47*
>
> "You have a right to the work, never to its fruits."

1. **Do the work well, regardless of outcome.** Ship quality. Let results follow.
2. **State assumptions explicitly.** Especially when extrapolating beyond known data.
3. **Prefer simple, legible systems** over clever ones. Future maintainers are not telepathic.
4. **Optimize for reversibility.** When an action is hard to undo, slow down and confirm.
5. **Disagree in writing, decide in writing.** Verbal alignment evaporates; written alignment compounds.
6. **No magical claims in code, docs, or marketing.** Describe what the system actually does.

---

## 3. Engineering Protocol

### 3.1 Repository hygiene

- All work lands on a feature branch and is merged via PR review.
- The default branch must always build and pass tests.
- Generated artifacts and secrets never enter the repo.

### 3.2 Code

- Names carry the meaning; comments explain the *why* when it is non-obvious.
- Every public interface has at least one test exercising its contract.
- Dependencies are added deliberately, with a one-line justification in the PR.

### 3.3 Review

- Reviews check correctness, security, and clarity — in that order.
- A reviewer who blocks must propose a path to unblock.
- Approvals are for the diff seen, not for future changes.

### 3.4 Operations

- Anything user-facing has a rollback plan before it ships.
- Incidents are followed by a written postmortem within one week.
- We do not bypass safety hooks (`--no-verify`, force pushes to protected branches, etc.) without explicit, recorded authorization.

---

## 4. Decision Framework

When facing a non-trivial decision, answer in order:

1. **What problem are we solving?** State it in one sentence.
2. **What changes if we do nothing?** If little changes, consider not acting.
3. **What is the smallest reversible step that tests the hypothesis?**
4. **What evidence would tell us we were wrong?**
5. **Who is affected, and have they been informed?**

Record the answers alongside the change. The record is the artifact; the decision is downstream of it.

---

## 5. Roles

- **Maintainer:** Holds the merge bit. Responsible for branch health and release cadence.
- **Contributor:** Proposes changes via PR. Owns the change through review and rollout.
- **Reviewer:** Reads with intent to understand. Approves, requests changes, or escalates.
- **Operator:** Runs the system in production. Has authority to roll back without approval.

These roles rotate. None of them are titles.

---

## 6. Communication

> *सत्यं ब्रूयात् प्रियं ब्रूयात् न ब्रूयात् सत्यमप्रियम्।*
>
> *— Manusmṛti 4.138 (traditional)*
>
> "Speak the truth, speak it kindly; do not speak truth that wounds without cause."

- Be direct. Be kind. Both, not either.
- Default to public channels; reserve private channels for genuinely private matters.
- When you don't know, say so. "I don't know yet" is a complete answer.

---

## 7. What This Project Is Not

To prevent drift, it is worth stating plainly:

- It is **not** a substitute for professional, medical, legal, or spiritual counsel.
- It is **not** a vehicle for unverifiable claims about consciousness, physics, or metaphysics presented as engineering output.
- It is **not** a hierarchy in which any contributor is required to "align" beyond the written norms in this document.

People work here because the work is good. That is the only leverage we use.

---

## 8. Amendments

This document changes by pull request, like the code. Substantive changes require:

1. A written rationale in the PR description.
2. Review by at least one maintainer other than the author.
3. A note added to the changelog below.

### Changelog

- **2026-05-12** — Initial version of the Master Command established on `claude/build-x9elysium-master-xQOrp`.

---

> *सर्वे भवन्तु सुखिनः सर्वे सन्तु निरामयाः।*
> *सर्वे भद्राणि पश्यन्तु मा कश्चिद्दुःखभाग्भवेत्॥*
>
> "May all be well, may all be free from affliction, may all see what is good, may none suffer."
