# Blueprint AI Document Standards

**Version:** Genesis 0.3  
**Status:** Foundational  
**Purpose:** Define how Blueprint AI documents should be written, organized, and maintained.

---

## 1. Document Purpose

Every document must have a clear reason to exist.

At the top of each major document, include:

```text
# Document Title

Version:
Status:
Purpose:
```

Recommended status labels:

- Draft
- Working
- Foundational
- Active
- Deprecated
- Archived

---

## 2. Plain Language Rule

Blueprint AI documents should be understandable by business owners, consultants, team members, and AI systems.

Use clear language. Avoid jargon unless the term is defined.

---

## 3. Structure Rule

Use headings to make documents scannable.

Preferred structure:

```text
# Title

Version:
Status:
Purpose:

---

## 1. Main Section

### 1.1 Subsection
```

Numbered headings are preferred for core framework documents because they make references easier.

---

## 4. Separation Rule

Keep universal framework content separate from business-specific implementation content.

Use:

```text
kernel/
```

for reusable rules and logic.

Use:

```text
templates/
```

for reusable blanks and document formats.

Use:

```text
playbooks/
```

for step-by-step procedures.

Use:

```text
implementations/[business-name]/
```

for a specific business.

---

## 5. AI Readiness Rule

Documents should be easy for AI systems to read and act on.

Use:

- Clear headings
- Lists where useful
- Stable names
- Consistent labels
- Explicit definitions
- Concrete instructions
- Minimal ambiguity

Avoid burying important instructions in long paragraphs.

---

## 6. Business Reality Rule

Documents should reflect the business as it is, then clearly distinguish future plans.

Use labels such as:

```text
Current Reality:
Planned Improvement:
Future Possibility:
Open Question:
```

This prevents confusing existing operations with ideas that have not yet been implemented.

---

## 7. Versioning Rule

When a document changes meaningfully, update the relevant changelog or case study notes.

A meaningful change includes:

- A new operating rule
- A new template
- A new playbook
- A new business implementation insight
- A major correction
- A strategic shift

---

## 8. File Naming Rule

Use clear uppercase names for major foundation documents:

```text
NORTH_STAR.md
MASTER_PHILOSOPHY.md
MASTER_BLUEPRINT.md
```

Use descriptive uppercase names for kernel documents:

```text
OPERATING_MODEL.md
DECISION_RULES.md
DOCUMENT_STANDARDS.md
```

Use descriptive template names ending in `_TEMPLATE.md`:

```text
BUSINESS_PROFILE_TEMPLATE.md
IMPLEMENTATION_BRIEF_TEMPLATE.md
```

Use descriptive playbook names ending in `_PLAYBOOK.md`:

```text
FIRST_IMPLEMENTATION_PLAYBOOK.md
```

---

## 9. Change Safety Rule

Do not casually overwrite foundational documents.

When changing a foundational document, ask:

- Does this improve the framework?
- Does this conflict with existing principles?
- Should this be a new document instead?
- Should this be implementation-specific instead?

---

## 10. Documentation Standard

A Blueprint AI document is successful when it can help someone else continue the work without losing the purpose, reasoning, or direction of the project.
