# GitHub Setup Guide

You do not need to know Git or use the command line to use this governance process. GitHub has a web interface that handles everything described here.

This guide is an implementation guide for GitHub specifically. The governance principles in Two's Company Kit work on any platform that provides shared access, version history, identifiable authorship, review and approval, and retained records. If you use a different platform, apply the same principles there.

---

## Section 01. Key concepts

**Repository (repo).** A folder that holds your project files and their version history. Git records committed changes and makes earlier versions recoverable.

**Branch.** A separate copy of the repo where you can make changes without affecting the main version. Think of it as a draft.

**Main branch.** The official, current version of the project. Changes go here only after review.

**Pull request (PR).** A proposal to merge changes from a branch into main. The other collaborator can see exactly what changed, discuss it, and approve or request changes before it's merged.

**Review.** Looking at a proposed change and approving it, requesting changes, or commenting. This is the governance mechanism: material changes don't happen without someone else looking at them.

**Merge.** Accepting a proposed change into the main branch. Once merged, it's part of the official version.

**Issues.** A way to track tasks, bugs, questions, or proposals. Each issue has a discussion thread.

**Branch protection (rulesets).** Rules that can restrict certain actions on the main branch, like requiring PR reviews before merging. Available controls depend on your repository type and GitHub plan.

**CODEOWNERS.** A file that tells GitHub which people should be treated as responsible reviewers for specific parts of the project. CODEOWNERS does not prevent someone from changing a file. It ensures the designated reviewer is notified and, where branch rules require it, asked to approve. Important: CODEOWNERS uses "owner" to mean review responsibility. It does not determine intellectual property ownership. Someone listed as a code owner for `/src/` is the person GitHub asks to review changes there, not necessarily the person who owns the IP in that code. IP treatment is a governance decision recorded in [02 Who Owns What](../02-who-owns-what.md) and the [Working Agreement](../templates/working-agreement.md).

---

## Section 02. Access, responsibility, approval authority, platform role, and IP treatment

These are five different things. Confusing them is one of the most common governance mistakes.

**Access** is what someone has permission to do in the repository. Can they read it? Push code? Change settings? Access is a technical permission.

**Responsibility** is who is accountable for maintaining or reviewing a part of the project. This is not the same as IP treatment.

**Approval authority** is who has the standing to approve a change. Someone might have permission to edit the repository but not be the designated reviewer for financial logic. Someone might maintain the app code but not have authority to change the revenue split. Someone might be a CODEOWNERS entry for a source file but not have access to the payment platform.

**Platform role** (for example, Owner in a GitHub organization) is what administrative permissions the platform itself gives you. Owner is the highest administrative role in a GitHub organization: it can manage settings, billing, and access. This is an administrative role, not an IP or governance designation. Where the project uses a GitHub organization, giving both collaborators the Owner role avoids a single-person dependency. This recommendation applies to a GitHub organization specifically, not to every platform, and not to accounts that are identity-bound.

**IP treatment** is who is intended to have what rights in the asset. This is a governance decision the collaborators make and record in [02 Who Owns What](../02-who-owns-what.md) and the [project asset inventory](../templates/project-asset-inventory.md). No platform setting determines it.

CODEOWNERS uses "owner" to mean review responsibility. It does not determine intellectual property ownership.

Keep these distinct. The [access and custody matrix](../templates/access-and-custody-matrix.md) tracks access. The [Working Agreement](../templates/working-agreement.md) tracks decision rights and authority. CODEOWNERS tracks review responsibility. [02 Who Owns What](../02-who-owns-what.md) and the [project asset inventory](../templates/project-asset-inventory.md) track intended IP treatment.

---

## Section 03. Getting started

These three levels build on each other. Start with Level 1. Move to Level 2 when the project has distinct responsibility areas. Most two-person projects won't need Level 3 right away.

Both collaborators should record their GitHub usernames in the [project directory](../templates/project-directory.md). CODEOWNERS, @mentions in issues and PRs, and commit history all rely on knowing who's who on the platform.

---

## Section 04. Level 1: Don't lose each other's work

This is the minimum. Two collaborators, one shared workspace.

### 4.1 Create a shared GitHub organization

Create a shared GitHub organization and choose the plan that fits the project. Name it something neutral or project-specific. Add both collaborators as owners.

Why an organization instead of a personal account: if either collaborator leaves, the other still has full access. No single-person dependency.

### 4.2 Create the repository

Inside the organization, create a new repository. Initialize it with a README. Do not choose a license just because Two's Company Kit uses one. Your shared project's license is a separate decision. If you have not deliberately chosen a license for your project, you can leave that option blank for now.

### 4.3 Use pull requests for meaningful changes

Agree as a governance rule that material changes go through pull requests. One collaborator proposes, the other reviews, then merge. This creates a timestamped, reviewable record of the changes proposed through that process and who reviewed them.

### 4.4 Review each other's work

Before merging a PR, the other collaborator looks at it. This is the simplest governance mechanism: somebody besides the author saw the change before it took effect.

### 4.5 Enable MFA

Both collaborators should enable two-factor authentication on their GitHub accounts. Security baseline.

### 4.6 Record access

Fill in the source control row in the [access and custody matrix](../templates/access-and-custody-matrix.md).

---

## Section 05. Level 2: Know who's responsible for what

As the project grows or responsibilities become more distinct.

CODEOWNERS availability depends on your repository's visibility and plan. Before relying on it, open the file on GitHub and confirm it loads without errors. If it doesn't, keep the review responsibility as a written governance rule instead: record who reviews what in your Working Agreement and follow it, even though GitHub isn't routing the request for you.

### 5.1 Add CODEOWNERS

Create a `CODEOWNERS` file that maps areas of the project to the collaborator responsible for reviewing changes there. For example, financial module changes should be reviewed by the collaborator who maintains the financial module. Governance document changes should be reviewed by core maintainers.

CODEOWNERS tells GitHub: "When somebody changes this part of the project, make sure this person sees it." It does not prevent changes. It ensures the right person is in the review loop.

A typical two-person collaboration might look like:

```
# Application code
/src/                    @builder-a

# Financial model
/finance/                @builder-b

# Governance records: both review
/governance/             @builder-a @builder-b

# CODEOWNERS itself: both review
/.github/CODEOWNERS      @builder-a @builder-b
```

Substitute real GitHub usernames. Even with only two people, this makes responsibility visible.

Two mechanics to know before you write rules that governance depends on.

**Order matters, and the last matching pattern wins.** GitHub reads the file top to bottom, but the last rule that matches a file is the one that applies. Put a broad catch-all first and more specific rules below it. A specific rule placed above the catch-all will be overridden by it.

**Multiple owners for one pattern must be on the same line.** If you list two owners for the same path on separate lines, only the last one applies. `/governance/ @builder-a @builder-b` assigns both. The same two names on consecutive lines assigns only `@builder-b`.

### 5.2 Protect the CODEOWNERS file

The CODEOWNERS file itself should go through the same review process as any other governance document. Otherwise someone can reassign review responsibility without the current reviewer knowing.

### 5.3 Document access separately

CODEOWNERS tracks review responsibility. The [access and custody matrix](../templates/access-and-custody-matrix.md) tracks who has what access to what systems. Keep both current.

---

## Section 06. Level 3: Enforce where available

Where your GitHub plan supports it, add technical enforcement.

### 6.1 Protect the main branch

GitHub can enforce rules such as requiring a pull request and review before changes reach main. Available controls depend on your repository type and GitHub plan, so check the current GitHub settings for your repository.

Where available, consider:

- requiring a pull request before merge
- requiring at least one review from the other collaborator
- blocking force pushes
- blocking deletion of main
- reviewing any bypass permissions so the enforcement matches what you intended

If your GitHub plan does not support these controls, use the same process as a governance rule even when GitHub cannot technically enforce it: make material changes through pull requests and have the other collaborator review them before merge.

### 6.2 Required CODEOWNERS review

Where branch rules support it, require approval from the designated CODEOWNERS reviewer before merging changes to their area.

One caveat if you write governance rules that depend on this. When several code owners are assigned to the same path, GitHub's required CODEOWNERS review is satisfied by approval from any one of them. It does not by itself enforce a governance rule requiring approval from every listed maintainer. Configure additional review requirements, or enforce that rule procedurally, where you need it.

### 6.3 Status checks

If the project has automated tests, require them to pass before merging.

---

## Section 07. Not using GitHub?

GitHub is a recommended implementation, not a governance requirement. Another tool works fine if it provides:

- Shared access for all collaborators
- Version and change history
- Identifiable authorship (who made each change)
- Review and approval before changes take effect
- Retained records

The governance process described in Two's Company Kit works on any platform that meets these criteria. The principles matter more than the platform.
