# Project Directory

Track the project's names, handles, URLs, identifiers, and locations in one place. This is the "what is it called and where is it" record.

The [access and custody matrix](access-and-custody-matrix.md) tracks who can access, control, and recover each system. The Project Directory tracks what the system is called and how to find it. Keep both current, but keep them separate.

**Never store passwords, API keys, MFA recovery codes, or other secrets in this directory.**

---

## Section 01. Project identity

| Field | Value |
|---|---|
| Project name | |
| Repository URL | |
| Primary domain (if any) | |
| Organization / workspace name | |
| Other public-facing names | |

---

## Section 02. Collaborator handles

Record each collaborator's usernames and handles across the services the project uses. This is needed for CODEOWNERS, @mentions, commit attribution, and knowing who's who.

| Service or context | Collaborator A | Collaborator B |
|---|---|---|
| GitHub username | | |
| Email (project use) | | |
| Payment platform | | |
| Domain registrar | | |
| Hosting platform | | |
| Communication (Slack, Discord, etc.) | | |
| Other: | | |

---

## Section 03. Project accounts and services

Where does the project live? Record the name, URL, and identifier for each service the project uses. For access, custody, and recovery information, see the [access and custody matrix](access-and-custody-matrix.md).

| Service | Account or workspace name | URL or identifier | Notes |
|---|---|---|---|
| Source control | | | |
| Domain / DNS | | | |
| Hosting / deployment | | | |
| Database / data store | | | |
| Payment / revenue platform | | | |
| Project email | | | |
| Shared documents / project management | | | |
| Analytics / monitoring | | | |
| Communication | | | |
| Other: | | | |

---

## Section 04. Review cadence

Update this directory when:

- A new service or account is added
- A service name, URL, or identifier changes
- A collaborator's handle changes
- A collaborator joins or exits

---

*This is a living record maintained separately from the Working Agreement. Store the completed directory in the project's chosen governance-record location.*
