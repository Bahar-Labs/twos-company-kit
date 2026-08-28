# Two's Company Kit

A lightweight governance kit for two people building something together. Governance exists to support what you're building, and Two's Company Kit exists to support both.

**Make the important decisions while the collaboration is still easy. If the project grows into something that needs lawyers, accountants, or a formal entity, you'll arrive with a record of what you built, what you intended, and how you got there.**

**New here?** [Start here](guides/getting-started.md).

---

## Section 01. What this kit is

Two's Company Kit helps collaborators make decisions, document intentions, preserve evidence, anticipate common problems, and recognize when they've outgrown an informal governance framework. It helps you decide and record how you intend assets to be treated. It does not determine ownership, rights, or legal obligations.

It's designed for two people who want to build something together and don't have a legal department, an accountant, or a formal business entity. The kit walks you through the conversations you need to have, gives you templates to record your decisions, and tells you when it's time to get professional help.

## Section 02. What this kit is not

Two's Company Kit is not legal advice. It is not a legal agreement generator. It does not provide entity-formation guidance, tax or accounting advice, jurisdiction-specific legal guidance, or jurisdiction-specific regulatory or compliance guidance. It is not a substitute for qualified professional advice. It is not a governance framework for mature organizations. It is not a guarantee that a collaboration will succeed.

The kit helps you think clearly and keep good records. What those records mean in your jurisdiction, for your tax situation, under your local laws, is a question for professionals who know your circumstances.

---

## Section 03. What's in the kit

```
twos-company-kit/
├── README.md                           ← you are here
├── LICENSE                             ← content license
├── CONTRIBUTING.md                     ← how to propose a module
├── GOVERNANCE.md                       ← how this kit governs itself
├── DESIGN-PRINCIPLES.md                ← standards for how Two's Company Kit makes recommendations
├── MAINTAINERS.md                      ← who maintains what
│
├── 01-the-handshake.md                 ← contribution inventory
├── 02-who-owns-what.md                 ← intended IP treatment
├── 03-money.md                         ← revenue models and distribution
├── 04-infrastructure-and-custody.md    ← where it lives, who controls it
├── 05-expenses.md                      ← shared costs vs personal overhead
├── 06-what-happens-when.md             ← failure modes, exits, and transitions
├── 07-working-agreement.md             ← capturing your decisions
├── 08-contribution-log.md              ← running record of who did what
│
├── guides/
│   ├── getting-started.md              ← start here: order of operations
│   └── github-setup.md                 ← plain-language GitHub walkthrough
│
├── templates/
│   ├── contribution-inventory.md       ← blank inventory for Section 01
│   ├── project-asset-inventory.md      ← asset tracking for Section 02
│   ├── project-directory.md            ← names, handles, URLs, and locations
│   ├── working-agreement.md            ← blank agreement for Section 07
│   ├── contribution-log.md             ← blank log for Section 08
│   ├── access-and-custody-matrix.md    ← infrastructure control record
│   └── module-cover-template.md        ← branded cover for module contributors
│
├── modules/
│   └── financial-foundations/          ← basic financial decision support
│       ├── README.md
│       ├── revenue-split-calculator.md
│       ├── expense-tracker.md
│       └── break-even-worksheet.md
│
└── .github/
    ├── CODEOWNERS                      ← review responsibility assignments
    └── PULL_REQUEST_TEMPLATE.md        ← governance checklist for changes
```

---

## Section 04. A key distinction

Two's Company Kit separates five concepts that are easy to confuse:

- **Access** -- Can I do it technically?
- **Responsibility** -- Am I accountable for maintaining or reviewing it?
- **Approval authority** -- Can I authorize the decision?
- **Platform role** (for example, GitHub Owner) -- What administrative permissions does the platform give me?
- **IP treatment** -- Who is intended to have what rights in the asset?

Keep these distinct. The [access and custody matrix](templates/access-and-custody-matrix.md) tracks access. The [Working Agreement](templates/working-agreement.md) tracks decision rights and authority. CODEOWNERS tracks review responsibility. [02 Who Owns What](02-who-owns-what.md) and the [project asset inventory](templates/project-asset-inventory.md) track intended IP treatment.

---

## Section 05. How to use it

**Getting your own copy:**
Read the numbered sections here on GitHub. When you're ready to fill something in, copy the templates you need into your own private repository or other access-controlled location. Don't fork this repository for that purpose. Forks of a public repository are public, and a fork's visibility can't be changed on its own, so a fork is not a safe place for completed governance records. See [Section 06](#section-06-store-completed-records-appropriately).

**Starting a new collaboration:**
Work through the [Getting Started guide](guides/getting-started.md). It walks you through the order of operations.

**Using just one piece:**
Every section stands alone. Need the IP decision framework but nothing else? Grab [02 Who Owns What](02-who-owns-what.md).

---

## Section 06. Store completed records appropriately

Two's Company Kit templates may contain financial terms, contact information, infrastructure details, access information, or other sensitive project data. Public projects should not automatically publish completed governance records. Store completed records in a private repository or another access-controlled location when appropriate. Never commit passwords, API keys, MFA recovery codes, banking details, private customer information, or other secrets to a repository, even a private one.

---

## Section 07. When this kit stops being enough

Reaching one of these triggers doesn't mean something is wrong. It means the collaboration has grown beyond what a lightweight governance kit is designed to handle. That's a good thing. Take the records you've built here to the appropriate professionals.

**Consider professional advice or formalization when any of these become material:**

- Meaningful or recurring revenue
- Ongoing profit sharing
- Significant jointly developed IP
- Collaborators located in different countries or jurisdictions
- Significant cross-border payments
- Outside investors or investment discussions
- Debt or substantial financial commitments
- Employees or contractors
- Customer, personal, sensitive, or regulated data
- Sale or licensing of the project
- Acquisition interest
- Exclusivity requests
- Non-compete or similar restrictions
- Material disagreements over ownership
- Material disagreements over money
- One collaborator wants to formalize the relationship
- The collaboration begins operating like an ongoing business

Ongoing joint commercial activity, profit sharing, and similar arrangements may have legal, tax, reporting, or business-structure consequences depending on the jurisdictions involved, even when nobody formally created an entity. The kit does not determine those consequences. When these triggers become relevant, the records you've kept here give professionals something concrete to work with.

---

## Section 08. The module system

The core kit covers governance fundamentals. Official Modules add optional depth in specific domains.

Official Modules are developed, commissioned, or deliberately adopted by the maintainers and maintained under the project's governance process. Because an Official Module appears under the Two's Company Kit name, the maintainers determine what substantive review is appropriate before adopting it.

**Current Official Modules:**

- **Financial Foundations** -- basic revenue, expense, and break-even decision support

Contributors and maintainers work from [DESIGN-PRINCIPLES.md](DESIGN-PRINCIPLES.md), the editorial and governance standards used to review Two's Company Kit content.

Two's Company Kit does not currently host a formal Community Modules program. If there is enough community interest, a separate community-contribution model may be introduced later. Ideas, corrections, and module proposals are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

**A note on "modules":** A module in your collaboration is an asset whose intended treatment is decided by the collaborators using this kit. A module contributed to Two's Company Kit itself is governed by [CONTRIBUTING.md](CONTRIBUTING.md) and the [LICENSE](LICENSE). These are different things with different governance paths.

---

## Section 09. Terminology

To keep things clear across the kit:

- **Collaborator** -- a person working on the shared project
- **Contributor** -- a person contributing content, tools, or modules to Two's Company Kit itself
- **Maintainer** -- a person responsible for ongoing upkeep of the kit or a module
- **Shared project** -- the thing collaborators are building together

---

## Section 10. Project credits

Two's Company Kit was built through three operating brands of 1521 Holdings LLC:

- **Fieldline GRC Services** -- governance methodology and framework design
- **Bahar Labs** -- repository stewardship and technical architecture
- **578 Productions** -- publishing, production design, and visual packaging

The entity routing itself is part of the proof of concept. The kit governs what it teaches.

---

## Section 11. License

Two's Company Kit is © 2026 1521 Holdings LLC and is licensed under CC BY-NC-SA 4.0 (Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International).

**Additional permission:** You may use and adapt Two's Company Kit internally to govern your own collaboration, including a collaboration or project operated for commercial purposes. This permission does not authorize selling, sublicensing, white-labeling, incorporating Two's Company Kit into a paid product or service, or otherwise commercially exploiting the Two's Company Kit content itself. Commercial uses outside this permission require separate authorization from 1521 Holdings LLC.

**Attribution:** Two's Company Kit must be attributed to its original authors. Using, adapting, or distributing Two's Company Kit without attribution, or presenting it as your own original work, violates the license.

The Two's Company Kit name and the names, logos, trademarks, and other brand assets associated with 1521 Holdings LLC, Fieldline GRC Services, Bahar Labs, and 578 Productions are not included in the CC BY-NC-SA 4.0 content license. Use of names as reasonably necessary to provide required attribution is permitted.

See [LICENSE](LICENSE) for licensing details.

---

## Section 12. Why this exists

Builder communities are full of people who make great things alone. The next step is making great things together. That step needs a governance layer, and most indie builders don't have one.

Two's Company Kit is the pit stop before the road trip. It keeps the engine running longer.
