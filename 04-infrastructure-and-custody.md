# 04 -- Infrastructure and Custody

Every project lives somewhere. Someone's source control account. Someone's hosting platform. Someone's domain registration. Someone's credit card.

Each of those "someones" is a single point of failure. If that person disappears, gets locked out of their account, or stops paying the bill, the project goes dark. For collaborators without a shared business entity, this is the most overlooked risk in any collaboration.

---

## Section 01. Four core principles

**Named accounts.** Each collaborator uses their own account wherever the platform supports it. Shared username/password logins make it impossible to track who did what and impossible to revoke one person's access without locking out the other.

**Least privilege.** Give each collaborator the access they need for their role. Not everyone needs admin on everything. A collaborator who writes content doesn't need database admin access. A collaborator who deploys doesn't need billing admin.

**Documented recovery or succession path.** For each system the project depends on, the collaborators should document how access would be recovered or transferred if the custodian became unavailable. Where the platform supports more than one recovery-capable person, that is usually the simplest answer. Some accounts are identity-bound and genuinely cannot have a second recovery-capable user. Payment platforms, some registrars, and services tied to a single verified identity are common examples. For those, document the succession path instead: who holds the account, what the remaining collaborator would need to do, what evidence exists that the account serves the project, and what the agreed handoff looks like. The requirement is a documented path, not a fixed number of people.

**Access, responsibility, and approval authority are three different things.** Access is what someone can technically do. Responsibility is what someone is accountable for maintaining. Approval authority is what someone can authorize. Keep them distinct in your records. Someone can have access without authority, and authority without day-to-day access.

---

## Section 02. Access and custody matrix

Fill out the [access and custody matrix template](templates/access-and-custody-matrix.md) together at the start. Update it whenever something changes.

The matrix records: what the system is, who the primary custodian is, what the recovery or succession path is, what access each collaborator needs, whether MFA is enabled, how credentials or recovery information can be located (never the secrets themselves), and what happens to access on exit.

---

## Section 03. Recommendations

**Shared source-control workspace.** Don't host the project under either collaborator's personal account. Most source control platforms offer team or organization accounts. Where the platform supports multiple administrators, giving both collaborators that role avoids a single-person dependency. Name the workspace something neutral or project-specific.

**Domain and DNS: pick one custodian, document transfer terms.** Registration usually sits with one person. Decide and record what the collaborators intend to happen to the domain if the registrant exits, and document the recovery path in the [access and custody matrix](templates/access-and-custody-matrix.md).

**Hosting and deployment: prefer platforms with team or org accounts.** Many hosting platforms offer team plans that let both collaborators deploy. If you're on a free tier tied to one person's account, document a migration plan.

**Database or data store: the project needs enough access, recovery capability, or documented succession planning to avoid a single-person dependency.** That does not require both collaborators to have unrestricted day-to-day admin access. Decide what each collaborator's role requires and grant that.

**Payment and revenue platform: this is where the money flows.** If project revenue is collected through one collaborator's account, document the collection arrangement, applicable deductions, and how agreed distributions are made. See [03 Money](03-money.md). Payment platforms are frequently identity-bound, so this is a common case for a documented succession path rather than shared recovery access.

**Credential or secrets management.** Use a shared secrets-management system or vault rather than exchanging passwords over chat. Record where secrets are managed in the access and custody matrix, never the secrets themselves.

---

## Section 04. Joiner, mover, leaver

### When someone joins the collaboration

Give only the access required for their role. Don't give infrastructure access merely because someone contributed something. Record access granted in the matrix.

### When responsibilities change

Reassess access. Remove permissions no longer required. Don't let permissions accumulate indefinitely.

### When someone exits

Revoke access promptly. Transfer controlled project assets per the [Working Agreement](07-working-agreement.md). Rotate shared secrets when necessary. Preserve required project records. Confirm handoff completion.

---

## Section 05. The bus factor

For every row in the matrix, ask: "If this custodian were suddenly unavailable, could the project survive?"

If the answer is no, you need either shared access or a documented recovery or succession path. This isn't paranoia. People get busy, change priorities, take new jobs, move countries. The mundane version of being suddenly unavailable is "got a full-time offer and went quiet for three months." Plan for that.

---

## Section 06. When the project has no money yet

Most collaborations start pre-revenue. Someone is paying for hosting, domain, and tools out of pocket. Someone paying project costs out of pocket can create an unrecorded financial expectation that is easy to ignore and hard to unwind later. See [05 Expenses](05-expenses.md) for how to handle pre-revenue infrastructure costs.
