# Two's Company Kit Design Principles

Two's Company Kit helps people make, record, and revisit important decisions about a shared project.

These principles guide contributors and maintainers when creating, reviewing, or changing Two's Company Kit content. They are not rules for the collaborations using it. They are rules for **the kit itself**: what the kit should recommend, what it should leave to collaborators, and how it should distinguish guidance from decisions.

When a proposed sentence, template field, default, example, or workflow is unclear, use these principles to decide whether it belongs.

> **Terminology:** In this document, **contributor** means a person contributing to Two's Company Kit itself. **Collaborator** means a person participating in the shared project being governed with the kit. See the [Terminology](README.md#section-09-terminology) section in the README.

---

## Section 01. Recommend process without manufacturing substantive outcomes

Two's Company Kit may recommend **how a decision is made**: who should participate, when approval should happen, what questions should be considered, what should be documented, and where the resulting record should live.

Two's Company Kit should not silently determine **what collaborators are entitled to, what anyone owns, what rights anyone has, what debts exist, what obligations exist between collaborators, or what legal consequences follow**.

A recommended approval process is not a determination of substantive rights.

### The core test

Before adding a substantive statement, ask:

**Is Two's Company Kit helping the collaborators make and record a decision, or is it making the decision for them?**

Then ask:

**If someone followed this sentence literally, could they reasonably believe they acquired a right, incurred an obligation, became entitled to money, transferred ownership, or received authority that they never expressly decided or independently obtained?**

If yes, rewrite it.

### The test applied

These are real failures from this kit's own review history, kept as reasoning rather than as vocabulary. Do not treat the failed phrasings as a blocklist to grep for. Later problems will use different words. Learn the pattern that produced them.

**Failed: language asserting an unrecorded financial obligation.**
Why it failed: it concluded that money was owed when the collaborators may have chosen a model where nothing is reimbursable at all.
Principle that catches it: Section 01, and the caution list in Section 12.
Better pattern: describe the risk of leaving an expectation undocumented, and point to where the collaborators record what they actually agreed.

**Failed: a reimbursement field pre-labeled as a balance due.**
Why it failed: a template field can assert an outcome just as effectively as a sentence, and this one presumed the reimbursement model.
Principle that catches it: Section 02, since an unlabeled default in a template becomes an unstated rule.
Better pattern: mark the field conditional, so it applies only if the collaborators adopted that model.

**Failed: stating that a module's creator holds it and the project receives a license.**
Why it failed: it decided the IP outcome rather than surfacing it as a decision, and creator status does not by itself establish who holds rights.
Principle that catches it: Section 01, with Section 05 where third-party material is involved.
Better pattern: offer the arrangement as a named starting point, say plainly that collaborators may choose differently, and route the actual answer to the asset inventory.

**Failed: characterizing a collection account as if it held someone else's money.**
Why it failed: it concluded an entitlement before any deductions, distribution terms, or right to payment had been decided.
Principle that catches it: Section 01, and Section 04 for treating account control as if it settled a rights question.
Better pattern: instruct collaborators to document the collection arrangement, applicable deductions, and how agreed distributions are made.

Two recommendations passed the same tests and were kept. Recommending that both collaborators approve a change to the revenue split shapes who participates in a decision without deciding what anyone receives. Recommending a module treatment as a labeled starting point offers a useful default while leaving the outcome open. The difference in every case is process versus outcome. Nothing else.

A repair is not a rule. When a similar problem appears in new words, work from the principle, not from the wording of a previous fix.

---

## Section 02. A default must announce itself as a default

Two's Company Kit may offer useful starting points. A starting point is not a determination.

When the kit recommends a default treatment, workflow, approval model, threshold, or other starting position:

- identify it as a recommendation, example, common approach, or starting point;
- explain why collaborators might find it useful when that context matters;
- make clear that collaborators may choose something different; and
- tell collaborators where to record the decision they actually make.

Do not allow a recommended default to become an unstated rule merely because it appears in a template.

---

## Section 03. The decision belongs in the record

Guidance helps collaborators reach a decision. Completed project records capture the decision.

Two's Company Kit explanatory content should not substitute for the collaborators documenting what they actually chose.

When a decision matters, direct collaborators to an appropriate durable record such as the Working Agreement, contribution inventory, project asset inventory, access and custody matrix, contribution log, or another identified project record.

The guidance may frame the question. The answer belongs to the collaboration.

---

## Section 04. Keep different kinds of authority separate

Two's Company Kit distinguishes concepts that are often collapsed into one another:

- **Access:** what someone can do technically.
- **Responsibility:** what someone is expected to maintain, review, or oversee.
- **Approval authority:** what decisions someone may authorize.
- **Platform role:** what permissions a service or platform assigns.
- **IP treatment:** what rights collaborators intend to apply to an asset.

Do not infer one from another.

Technical access does not create decision authority. Responsibility does not create ownership. A platform role does not determine IP rights. CODEOWNERS identifies review responsibility; it does not determine ownership.

Templates, examples, and guidance should preserve these distinctions.

---

## Section 05. Do not create rights that do not exist

Two's Company Kit can help collaborators identify and record rights available to them. It cannot enlarge those rights.

This is especially important for:

- third-party material;
- open-source software or content;
- licensed assets;
- contributor material;
- trademarks and brand assets;
- platform-controlled accounts or resources; and
- material subject to outside terms or agreements.

When an asset comes from outside the collaboration, Two's Company Kit should direct collaborators to identify the applicable license, terms, permission, or other source of rights and make their intended treatment consistent with what is actually available.

A record of intended treatment does not override third-party rights.

---

## Section 06. Keep examples from turning into requirements

Examples help people understand a concept. They should not quietly become mandatory architecture.

Vendor names, platforms, dollar amounts, approval thresholds, account structures, storage locations, workflows, revenue models, and similar examples should be clearly illustrative unless Two's Company Kit deliberately intends to recommend them.

Where a recommendation depends on an assumption, make the assumption visible.

Examples include assumptions such as:

- there are exactly two collaborators;
- both collaborators can technically access a system;
- a project uses GitHub;
- project revenue passes through one person's account;
- both collaborators are located in the same jurisdiction; or
- a particular recovery method is technically possible.

Do not allow an implementation example to masquerade as a governance rule.

---

## Section 07. Remain jurisdiction-neutral

Two's Company Kit is a lightweight governance kit, not jurisdiction-specific professional advice.

Do not silently import the legal rules, terminology, entity structures, tax treatment, employment concepts, accounting requirements, or regulatory assumptions of a particular jurisdiction.

Jurisdiction-neutral does not mean pretending jurisdiction does not matter. Where location or applicable law could materially change the answer, Two's Company Kit should identify the issue and direct collaborators toward appropriate professional advice rather than supplying a universal answer.

---

## Section 08. Do not confuse informality with absence of consequences

An informal collaboration can still create real legal, financial, tax, regulatory, operational, or business consequences.

Two's Company Kit should not assure collaborators that informality prevents those consequences. It should also not attempt to determine what those consequences are.

Instead, Two's Company Kit should:

- identify circumstances that may justify professional advice or formalization;
- help collaborators preserve useful records;
- make assumptions and unresolved questions visible; and
- stop short of conclusions outside the kit's scope.

The purpose of an escalation trigger is to recognize the boundary of the kit, not to diagnose what exists beyond it.

---

## Section 09. Use precise roles and terminology

Two's Company Kit uses specific terms deliberately.

A **collaborator** participates in the shared project being governed with Two's Company Kit.

A **contributor** contributes material, tools, or modules to Two's Company Kit itself.

A **maintainer** is responsible for ongoing upkeep of the kit or a module.

A **shared project** is the thing collaborators are building together.

Do not substitute these roles casually when the distinction affects rights, responsibilities, governance, attribution, or process.

A module created within a collaboration and a module contributed to Two's Company Kit are different things with different governance paths.

---

## Section 10. Preserve provenance and contributor identity

Two's Company Kit should make it possible to understand where material came from, who contributed it, and how it entered the project.

Contributor attribution should remain attached to contributed work as required by the project's contribution and licensing terms.

Contributor identity, attribution, branding, copyright, maintenance responsibility, and Two's Company Kit adoption are separate concepts. Do not treat one as automatically granting another.

Where Two's Company Kit permits contributor branding or other third-party material to accompany a contribution, the applicable contribution and licensing terms should clearly establish the permissions needed to publish, maintain, distribute, and archive that material.

---

## Section 11. Prefer durable evidence over memory

Important governance decisions should leave a record.

Where appropriate, Two's Company Kit should help collaborators capture:

- what was decided;
- who participated;
- who approved;
- when the decision occurred;
- what asset, account, expense, responsibility, or issue the decision concerned;
- what assumptions or conditions applied; and
- where the authoritative record lives.

The goal is not paperwork for its own sake. The goal is to make important decisions understandable later, especially after circumstances or memories change.

---

## Section 12. Use plain language without false certainty

Two's Company Kit should be understandable to people who are not lawyers, accountants, developers, or governance specialists.

Plain language does not require oversimplifying an uncertain question into a definitive answer.

Prefer language that accurately communicates the function of the kit:

- **helps decide**
- **helps record**
- **intended treatment**
- **recommended starting point**
- **consider**
- **if you adopt this approach**
- **record what you decide**

Be cautious with language that can imply an outcome already exists:

- **owns**
- **is entitled to**
- **is owed**
- **must**
- **creates a debt**
- **has authority**
- **transfers**
- **guarantees**

Those words may sometimes be correct. When they appear, contributors should be able to identify the decision, source of authority, applicable term, or established fact that supports them.

---

## Section 13. Know when Two's Company Kit should stop

Two's Company Kit should identify questions outside its competence instead of improvising answers.

This includes questions requiring jurisdiction-specific legal, tax, accounting, regulatory, employment, entity-formation, investment, or other qualified professional advice.

When Two's Company Kit reaches that boundary, the appropriate response is generally to:

1. identify the issue;
2. explain why it matters at a practical level;
3. preserve the relevant facts and decisions; and
4. recommend appropriate professional review.

Knowing where the kit stops is part of the design.

---

## Section 14. Review the system, not only the sentence

Two's Company Kit is a connected governance system.

A change that is correct in one file may still create a contradiction elsewhere. Substantive changes should therefore be reviewed across:

- explanatory sections;
- templates;
- guides;
- Official Modules;
- contribution terms;
- governance rules; and
- repository workflows where applicable.

When a principle or governance model changes, search for older language that may still encode the previous model.

Cross-file consistency is a governance requirement, not merely an editing preference.

### Record the reasoning, not the repair

When a fix is documented, record what failed, why it failed, which principle catches it, and what the better pattern is. Do not preserve the rejected wording as canonical vocabulary.

Two reasons. A maintainer who learns the repair applies it only to the exact words that produced it, and the next instance of the same problem will use different words. And rejected phrasings kept verbatim become live strings in the repository, which turns any search intended to catch a regression into a search that finds this document instead.

Describe the failure. Do not enshrine it.

---

## Section 15. Contributor review questions

Before proposing or approving substantive content, ask:

1. Is this guidance about **process**, or does it accidentally determine a substantive outcome?
2. If it is a default, have we clearly identified it as one?
3. Does the actual collaborator decision have a place to be recorded?
4. Are access, responsibility, approval authority, platform role, and IP treatment kept distinct?
5. Does this language assume rights that the collaborators may not possess?
6. Is an example accidentally functioning as a requirement?
7. Have we imported a jurisdiction-specific assumption?
8. Could this language be mistaken for professional advice?
9. Are contributor and collaborator roles being kept separate?
10. Does the statement use certainty that the source material does not support?
11. Does another file, template, guide, or module need to change with it?
12. Has Two's Company Kit reached a point where the right answer is to stop and route outward?

If the answer exposes an ambiguity, resolve it before merge.

---

## Section 16. The standard

Two's Company Kit should help people make important decisions earlier, make those decisions deliberately, and leave enough evidence to understand them later.

It should provide structure without pretending to provide rights, certainty, or professional conclusions that it cannot provide.

**Help collaborators decide. Help them record. Do not decide for them what only they, their circumstances, their existing rights, or qualified professionals can determine.**

Changes to this document are governance changes and follow the process in [GOVERNANCE.md](GOVERNANCE.md).
