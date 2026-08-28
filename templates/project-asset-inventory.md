# Project Asset Inventory

Record the assets the shared project depends on or whose treatment could matter later. This surfaces the questions Two's Company Kit is designed to help you answer: who created it, who holds it, where does it live, what's the intended treatment, and what happens to it on exit.

See [02 Who Owns What](../02-who-owns-what.md) for the decision framework. Reference this inventory in the [Working Agreement](working-agreement.md).

---

## Section 01. Asset types

Common types to consider (your project may have others):

- code
- content
- methodology / framework
- design / brand asset
- domain
- dataset / data
- financial model
- documentation
- account / infrastructure
- licensed third-party material
- other

---

## Section 02. Inventory

| Asset ID | Asset | Type | Existed before collaboration? | Created / brought by | Holder / custodian | Location / reference | Intended treatment | Project use rights | Post-exit treatment | Notes |
|---|---|---|---|---|---|---|---|---|---|---|
| A-001 | | | | | | | | | | |
| A-002 | | | | | | | | | | |
| A-003 | | | | | | | | | | |

**Asset ID:** Simple incrementing identifier (A-001, A-002, etc.). Use the ID to reference specific assets in the Working Agreement, exit checklist, contribution log, or other records.

**Created / brought by:** The collaborator who made or contributed this asset.

**Holder / custodian:** The collaborator (or account) that currently controls access to this asset. This may be a different person from the creator. Someone might build a financial model that lives in the other collaborator's repository. Someone might register a domain that the project depends on. This distinction matters.

**Location / reference:** Where the asset actually lives. The service names below are illustrative only, not recommendations; use whatever your project actually uses. For example: "Bahar-Labs/twos-company-kit repo," "Google Drive folder [name]," "Figma project [name]," "[registrar] account under [custodian]." If someone needs to find this asset six months from now, this column tells them where to look.

**Intended treatment:** How the collaborators intend this asset to be governed. For example:

- "Remains with creator; project has permission to use"
- "Jointly available to both collaborators"
- "Designated for shared project use, with custody held by [collaborator/account/entity]"

**Project use rights:** What the project can do with this asset. For example: "use and adapt within the project," "display but not modify," "redistribute under project license."

For licensed third-party material, record the applicable license or terms and make sure the project's intended treatment is consistent with the rights actually available under them. The collaborators' intentions cannot create rights the license does not grant. See [02 Who Owns What](../02-who-owns-what.md), Section 04.

**Post-exit treatment:** What happens to this asset if a collaborator exits. For example: "stays with creator, project retains permission to use existing version," "transfers to remaining collaborator," "reverts to creator." Reference the exit checklist in [06 What Happens When](../06-what-happens-when.md) for common scenarios.

**Notes:** May contain identifying/context information but **never passwords, API keys, recovery codes, or other secrets.**

---

## Section 03. Review cadence

Review the inventory when:

- A new asset is created or acquired that the project depends on
- An asset changes hands or storage location
- A collaborator exits
- The Working Agreement is updated

---

*This is a living record maintained separately from the Working Agreement. Changes to individual assets follow this inventory's own review process. Changes to the intended treatment framework require an update to the Working Agreement. Store the completed inventory in the project's chosen governance-record location.*
