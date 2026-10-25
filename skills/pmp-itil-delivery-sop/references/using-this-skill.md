# Using the PMP & ITIL Delivery SOP Skill

Use this reference only when the user needs help framing a request or selecting a workflow.

## Minimum useful input

The user can start with ordinary language. Extract what is present and ask only for missing details that change the next action:

- desired outcome and affected customer, user, or service;
- current situation and urgency;
- relevant commitment, deadline, constraint, or contract;
- decision owner or approval needed, if known;
- desired output: plan, meeting record, customer update, impact assessment, checklist, or decision advice.

Do not require every field. Clearly label unknowns and assumptions.

## Route the request

| User situation | First route | Typical output |
|---|---|---|
| New initiative or customer ask | Intake and initiation | One-page intake, scope boundary, risks, first customer message |
| Work already in progress | Delivery and control | Status update, action/risk/issue/decision log |
| New customer need | Backlog or change routing | Backlog vs. change decision, impact assessment, recommendation |
| Service is unavailable or degraded | Incident management | Restore-first actions, stakeholder update, escalation decision |
| Failure repeats or has unknown cause | Problem management | Problem record, root-cause work, workaround and improvement plan |
| Release or handover is approaching | Transition to service | Readiness and handover checklist, owners, open gaps |
| Work is complete | Closure and improvement | Acceptance, closure actions, lessons learned, improvement item |

## Copyable prompt patterns

### Start a project

```text
Use $pmp-itil-delivery-sop. I need to start [initiative].
The customer outcome is [outcome]; target date or constraint is [constraint].
Known stakeholders are [people/roles].
Create a one-page intake, initial risks, and a first customer-alignment message.
```

### Run a weekly review

```text
Use $pmp-itil-delivery-sop. Here is this week's project/service status: [facts].
Turn it into a concise review: delivered value, next commitments, risks, current issues, decisions needed, owners, and customer update.
```

### Handle a new request or change

```text
Use $pmp-itil-delivery-sop. The customer requests [request].
The current agreed scope/commitment is [commitment], and the likely impact is [known impact].
Decide whether this belongs in the backlog or needs a controlled change. Draft the impact assessment and recommended customer response.
```

### Handle an incident

```text
Use $pmp-itil-delivery-sop. Since [time], [service] has been [unavailable/degraded].
Affected users and business impact are [impact]; known facts are [facts].
Give restore-first actions, a customer update, escalation criteria, and whether to create a problem record.
```

### Prepare release and handover

```text
Use $pmp-itil-delivery-sop. [Service/project] is planned to go live on [date].
Current readiness is [facts]. Create a handover checklist, identify gaps, owners, approvals, validation, and rollback needs.
```

### Close and improve

```text
Use $pmp-itil-delivery-sop. [Initiative] is complete. Evidence and unresolved items are [facts].
Create acceptance/closure actions, lessons learned, and measurable continual-improvement items.
```
