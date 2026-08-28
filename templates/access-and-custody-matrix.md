# Access and Custody Matrix

Record every system the shared project depends on. Update whenever access changes. See [04 Infrastructure and Custody](../04-infrastructure-and-custody.md) for principles and guidance.

---

## Section 01. Systems

| System | Purpose | Primary custodian | Recovery custodian / succession path | Access each collaborator needs | MFA enabled? | Recovery method/location | Exit action |
|---|---|---|---|---|---|---|---|
| Source control | | | | | | | |
| Domain/DNS | | | | | | | |
| Hosting/deployment | | | | | | | |
| Database/data store | | | | | | | |
| Payment/revenue platform | | | | | | | |
| Project email | | | | | | | |
| Shared documents/project management | | | | | | | |
| Analytics/monitoring | | | | | | | |
| Backups/storage | | | | | | | |
| Production APIs/integrations | | | | | | | |
| Other: | | | | | | | |

**Recovery method/location:** Record where the secret is stored, never the secret itself. For example: "recovery codes in shared vault under 'ProjectName DNS'" rather than the actual codes.

---

## Section 02. Principles checklist

- [ ] Each collaborator uses their own named account where supported
- [ ] Access granted matches each collaborator's role (least privilege)
- [ ] Recovery or succession path documented for each critical system
- [ ] MFA enabled where supported
- [ ] Identity-bound accounts identified, with a documented succession path where a second recovery-capable user is not possible
- [ ] Exit actions defined for every system

---

*Store the completed matrix in the project's chosen governance-record location. Review when access changes or a collaborator exits.*
