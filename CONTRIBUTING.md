# Contributing

Two's Company Kit welcomes ideas, corrections, and proposals for new modules. This guide covers how to propose and contribute.

> **Terminology:** In this document, **contributor** means a person contributing to Two's Company Kit itself. **Collaborator** means a person participating in the shared project being governed with the kit. See the [Terminology](README.md#section-09-terminology) section in the README.

---

## Section 01. Rights and licensing

The Two's Company Kit core is © 2026 1521 Holdings LLC and is licensed under CC BY-NC-SA 4.0.

If you contribute original material to Two's Company Kit, you retain copyright in your contribution unless you and 1521 Holdings LLC separately agree otherwise. By submitting a contribution for inclusion in Two's Company Kit, you confirm that you have the right to contribute it and grant 1521 Holdings LLC a non-exclusive license to reproduce, adapt, maintain, distribute, and include the contribution as part of Two's Company Kit under the project's applicable license and the additional permissions stated in the repository LICENSE at the time of contribution.

Your attribution as the original contributor will be preserved for as long as your contribution remains part of Two's Company Kit, including in project history if it is later revised or archived.

Contributing to Two's Company Kit does not transfer ownership of your underlying expertise, knowledge, independently developed methods, tools, courses, services, or other work. For example, contributing a financial-planning worksheet does not prevent you from independently developing or selling your own financial-planning products or services.

Contributor names, logos, trademarks, and brand assets remain the property of the contributor and are separate from the Two's Company Kit content license.

### Brand-use permission for contributed material

Some contributions include contributor branding, for example a module cover page using the [module cover template](templates/module-cover-template.md). If you include your name, logo, trademark, or other brand asset with a contribution, you grant 1521 Holdings LLC a non-exclusive, royalty-free permission to reproduce, display, distribute, and archive that brand asset as part of Two's Company Kit and in materials describing Two's Company Kit.

This permission is limited to that purpose. It does not transfer ownership of your marks, does not permit standalone use of your marks apart from your contribution, does not create a general endorsement or partnership, and does not permit use of your marks to promote unrelated products or services.

You may withdraw this permission for future distributions by opening an issue. Copies already distributed and the project's history and archives are not affected, since attribution and provenance are preserved for as long as the contribution remains part of the kit.

If you have questions about the rights associated with a contribution, ask before contributing.

---

## Section 02. Official Modules vs. community contributions

A module proposal does not automatically become an Official Module.

Official Modules are developed, commissioned, or deliberately adopted by the maintainers and maintained under the project's governance process. Because an Official Module appears under the Two's Company Kit name, the maintainers determine what substantive review is appropriate before adopting it.

Two's Company Kit does not currently host a formal Community Modules program. If there is enough community interest, a separate community-contribution model may be introduced later.

---

## Section 03. What makes a good module proposal

Before proposing substantive content, read [DESIGN-PRINCIPLES.md](DESIGN-PRINCIPLES.md). It defines the editorial and governance standards used to review Two's Company Kit content.

A good module adds depth in a specific domain that the core kit doesn't cover. It should be useful on its own, grounded in real expertise, actionable (templates, worksheets, decision frameworks, not essays), and something you're willing to maintain.

### Examples of modules that could add value

- Financial scenario planning, budgeting, runway, and cash-flow decision tools
- Project management frameworks for async or remote collaborations
- Conflict resolution and mediation frameworks
- Technical architecture patterns for shared infrastructure
- Design system collaboration guidelines

### What is out of scope

Two's Company Kit does not accept modules that provide:

- Entity-formation determinations
- Determinations that a legal partnership, employment, or entity relationship exists
- Professional advice presented as universally applicable
- Content outside the kit's collaboration-governance purpose

Two's Company Kit also does not accept jurisdiction-specific modules. This includes, but is not limited to:

- Jurisdiction-specific legal advice or templates
- Jurisdiction-specific tax advice
- Jurisdiction-specific regulatory requirements
- Jurisdiction-specific accounting guidance

---

## Section 04. Module structure

Every module lives in its own directory under `/modules/`.

```
modules/
└── your-module-name/
    ├── README.md              ← required
    ├── [content files]        ← required as applicable
    └── cover.md               ← optional
```

### Module README should include

- Module name and one-line description
- Who it's for (which type of collaboration benefits)
- What's included (list of files and what each does)
- How to use it
- Scope and exclusions (what the module does not cover)
- About the contributor (name, entity, what you do, links)
- Author, maintainer, status, and last substantive review date
- License (same as the kit's content license)

### Module cover page (optional)

If you'd like to brand your module, use the template at [templates/module-cover-template.md](templates/module-cover-template.md). This is where your brand identity goes: your colors, your logo, your tagline. The 578 Productions design system provides the structural template. You provide the identity.

---

## Section 05. How to contribute

### Step 1: Open an issue

Before building, open a GitHub issue titled "Module proposal: [your module name]" with what the module covers, why it's needed (what gap it fills), your background, and an estimated timeline. This starts a conversation.

### Step 2: Agree on the contribution path

Before substantial work begins, the maintainers will decide whether the proposal is:

- appropriate for development as an Official Module;
- better suited to a contribution to an existing module;
- better suited to a future Community Module model; or
- outside the scope of Two's Company Kit.

This decision happens before you build, not after. If the proposal is accepted as an Official Module path, the maintainers and contributor agree on scope, structure, and review expectations.

### Step 3: Build

Once the contribution path is agreed, fork the repo. Create your module directory under `/modules/`. Build your content following the structure above.

### Step 4: Submit a pull request

PR title: "Add module: [your module name]." Include a link to the original issue, a summary of what's included, and your preferred attribution (name, entity, links).

### Step 5: Review and merge

Core maintainers review for fit, scope, structural consistency, adherence to the out-of-scope boundaries, licensing compatibility, attribution, and maintenance expectations. Because an Official Module appears under the Two's Company Kit name, the maintainers determine what substantive review is appropriate.

Core review does not constitute independent professional validation, certification, legal review, tax or accounting review, warranty, or endorsement of a contributor's services.

### Step 6: You're listed

Once merged, your module appears in the README under Official Modules. Your bio goes in the module README. You're a contributor.

---

## Section 06. After your module is merged

You maintain it. Issues and PRs against your module are your responsibility. You can propose updates anytime via PR. Your attribution is permanent, even if the module is later archived. You can share and promote it. It's your work. The kit gives it a home.

See MAINTAINERS.md for how maintainer status and succession work.

---

## Section 07. Questions?

Open an issue. Maintainer response expectations are documented in [MAINTAINERS.md](MAINTAINERS.md). We want good modules. The kit gets better when domain experts bring their knowledge to it.
