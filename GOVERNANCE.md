# Governance

How Two's Company Kit governs itself. If the kit asks collaborators a governance question, the kit should have an answer to the same question about itself.

> **Terminology:** In this document, **contributor** means a person contributing to Two's Company Kit itself. **Collaborator** means a person participating in the shared project being governed with the kit. See the [Terminology](README.md#section-09-terminology) section in the README.

---

## Section 01. What constitutes the core kit

The core kit is Sections 01 through 08, the README, this governance document, [DESIGN-PRINCIPLES.md](DESIGN-PRINCIPLES.md), [MAINTAINERS.md](MAINTAINERS.md), [CONTRIBUTING.md](CONTRIBUTING.md), the [LICENSE](LICENSE), the guides directory, and the templates directory. Changes to core kit content follow the change classifications in Section 04. Governance changes require core maintainer approval.

## Section 02. What constitutes an Official Module

An Official Module is a module the maintainers have deliberately adopted and agreed to maintain under this governance process. A third-party proposal or pull request does not become Official merely by being submitted. The maintainers determine what substantive review is appropriate before adopting a module under the Two's Company Kit name.

Financial Foundations is the initial Official Module.

## Section 03. Decision authority

Core maintainers have authority over the core kit. Module maintainers have authority over their modules, subject to the kit's scope and contribution guidelines. See [MAINTAINERS.md](MAINTAINERS.md) for the current list.

## Section 04. How material changes are proposed

Material changes to the core kit or Official Modules should be proposed through a pull request. The PR should describe what changed, why, and whether the change affects intended asset treatment, money, access, responsibilities, or governance.

Changes to `.github/CODEOWNERS` are governance changes and follow the governance-change process below.

[MAINTAINERS.md](MAINTAINERS.md) records who holds maintainer responsibility. `.github/CODEOWNERS` implements review routing for that responsibility on GitHub. If the two disagree, MAINTAINERS.md governs and CODEOWNERS is corrected to match.

### Operational changes

Updates within an assigned area of responsibility: fixing a typo, clarifying language, updating a link. Can be made by the responsible maintainer.

### Governance changes

Changes that affect intended asset treatment, revenue, scope, access, contributor terms, exit terms, governance rules, review responsibility assignments, or maintainer roles. Governance changes require approval by all other active core maintainers before merge. When Two's Company Kit has only one core maintainer, the change should still be made through a pull request so the proposal, rationale, and resulting change are recorded; independent approval is not implied.

## Section 05. Module adoption and removal

New modules are proposed through [CONTRIBUTING.md](CONTRIBUTING.md). The maintainers decide whether a proposal is appropriate for Official Module status before substantial work begins. Modules may be archived if unmaintained (see [MAINTAINERS.md](MAINTAINERS.md) for the process). Archived modules retain their original attribution.

## Section 06. Contributor boundaries

Substantive contributions must conform to [DESIGN-PRINCIPLES.md](DESIGN-PRINCIPLES.md) in addition to falling within the kit's scope (see [CONTRIBUTING.md](CONTRIBUTING.md) for what's in and out of scope). A change that fails either test in Section 01 of that document should not merge, including one written by a maintainer. The kit does not accept modules that provide jurisdiction-specific legal advice, entity-formation determinations, jurisdiction-specific tax advice, or professional advice presented as universally applicable.

## Section 07. Licensing and provenance

Contributors confirm they created the material or otherwise have the right to contribute it under the kit's license, including any additional permissions the project grants to users. See [CONTRIBUTING.md](CONTRIBUTING.md) for the full contributor rights section.

## Section 08. Maintainer succession

If a core maintainer becomes unavailable, the remaining core maintainer(s) may appoint a successor. If all core maintainers become unavailable, the project may be forked and continued subject to the applicable license terms and required attribution.

## Section 09. Escalation for sensitive or high-risk content

If proposed content touches legal, tax, financial, or regulatory topics in ways that could be mistaken for professional advice, core maintainers should flag it for additional review before merging.

## Section 10. How governance itself changes

Changes to this document are governance changes and follow the governance-change approval process described above.
