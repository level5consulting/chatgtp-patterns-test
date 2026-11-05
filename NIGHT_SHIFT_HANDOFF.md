# The Night Shift — AI Workflow Handoff Record

**AI Success Patterns — Ghost in the Workflow**

**Version:** Draft 1.0  
**Record created:** November 5, 2026  
**Documentation type:** FULL  
**Environment:** ChatGPT  
**Status:** Tested through simulation; production execution not verified

> TEST RECORD. This file documents the Night Shift simulation and intended policies, not a live production deployment. The repository is public; do not include confidential information.

## 1. Purpose

The Night Shift prepares and performs approved work during unattended periods, producing drafts, findings, and recommendations for later human review.

The workflow may perform authorized actions within established boundaries, while reserving publishing, deletion, and sensitive changes for human approval.

## 2. Owner

**Individual workflow creator**

Each creator is responsible for maintaining the documentation for the workflow they build.

**[Inferred — confirm]** The creator also coordinates reviews and transfers responsibility when ownership changes.

## 3. How to use it

### Inputs

- Approved work items and expected deliverables
- Authorized data sources
- Execution instructions and safety boundaries
- Defined human approval requirements

### Execution steps

1. Identify tasks suitable for unattended execution.
2. Prepare individual work briefs defining inputs, outputs, and restrictions.
3. Execute work using approved ChatGPT capabilities.
4. Preserve completed work and record exceptions.
5. Present results for morning review.
6. Have the human approve, change, or reject proposed actions.

### Simulation performed

Three jobs were tested:

| Job | Human decision | Result |
|---|---|---|
| Repository documentation | Change | Shakespeare-style README revision drafted, not published |
| Steering committee update | Approve | Draft accepted for use, not distributed |
| AI adoption risk review | Reject | Proposed risk not added to a live register |

**Expected output:** Completed drafts, findings, exceptions, and a human decision dashboard.

No real unattended execution occurred.

## 4. Depends on

**Confirmed:**
- ChatGPT as the intended execution environment
- GitHub repositories
- Files and documents
- Individual workflow ownership
- Human approval for specified actions

**Unknown or unverified:**
- Actual scheduling and unattended execution mechanism
- Connected-system permissions
- Technical enforcement of access limits
- Logging and monitoring capabilities
- Recovery procedures after interrupted execution

Implementation must be validated before production use.

## 5. Can reach

### Intended access

| Action | Policy |
|---|---|
| Read approved repositories | Permitted |
| Read approved files and documents | Permitted |
| Create or update files in designated locations | Permitted |
| Publish or distribute information | Human approval required |
| Delete records | Human approval required |
| Make sensitive changes | Human approval required |
| Access other systems | Not authorized |

These are intended policies, not verified technical controls.

The exact approved repositories, file locations, and authorization mechanism remain unspecified.

Do not place passwords, access keys, or other secrets in this record.

## 6. Decisions and rejected approaches

**Confirmed design decisions:**

- The individual workflow creator owns the workflow.
- ChatGPT is the selected execution environment.
- GitHub and files/documents are intended access categories.
- Write permissions are limited to designated locations.
- Publishing, deletion, and sensitive changes require human approval.
- A failed job stops, preserves safe completed work, and reports the error.
- Other independent jobs continue when one job fails.
- Reviews occur quarterly and after major changes.

**Simulation decisions:**

- The README was revised rather than accepted unchanged.
- The steering committee report was approved.
- The proposed risk recommendation was rejected.

**Rejected approach:** Automatically acting on all generated recommendations without human review is inconsistent with the confirmed approval policy.

No prior production implementation or alternative architecture has been established as tested and rejected.

## 7. Known limits

- Actual unattended execution has not been demonstrated.
- Scheduling and integration permissions remain unverified.
- AI output may contain inaccuracies or unsupported assumptions.
- Human approval is required before consequential actions.
- Technical enforcement of job isolation has not been tested.
- Logging, failure reporting, and restart behavior require validation.

**Failure handling:**

When a job fails, stop the affected job, preserve safe completed work, and report the error. Do not take further actions on that job. Allow independent jobs to continue.

**[Inferred — confirm]** Jobs dependent on failed output should not proceed until their dependency is resolved.

## 8. Review

**Required schedule:** Quarterly and after major changes.

**Initial record date:** November 5, 2026  
**Last production operational review:** Not established  
**Next scheduled review:** February 5, 2027, if the quarterly cycle starts from the initial record date. **[Inferred — confirm]**

Major changes triggering additional review include changes to the AI model, execution instructions, connected systems, access permissions, ownership, or approval rules.

## Maintenance instructions

When the workflow changes, update this handoff record in the same working session.

Keep it alongside the workflow or in an explicitly linked documentation location so future maintainers can find it.

**Permanent test storage location:** `level5consulting/chatgtp-patterns-test/NIGHT_SHIFT_HANDOFF.md`.

---

*This record describes the tested simulation and intended operating policies. It does not certify that the production workflow is deployed or safe to execute unattended.*
