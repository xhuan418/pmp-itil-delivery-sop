# Management Tool Selection Guide

Use this reference to turn a management question into a decision-ready table, chart, technique, or metric. Select the minimum tool that helps someone decide or act; do not produce a dashboard merely because data exists.

## First: identify the question

| Management question | Primary tool | Use it to decide |
|---|---|---|
| What exactly is included and accepted? | Scope statement + WBS, or product backlog + acceptance criteria | What is in/out and what “done” means |
| Who owns a decision or activity? | RACI / responsibility matrix | Who decides, does, advises, and receives updates |
| What can prevent the objective? | Risk register + probability-impact matrix | Prevention, contingency, owner, escalation |
| What is happening now and what needs attention? | RAID log + action/decision log | Priority, owner, due date, and decision needed |
| Is work late and where is recovery possible? | Milestone plan + dependency map / critical path | Which delay affects the finish date and which actions protect it |
| Is an agile iteration flowing as expected? | Burnup/burndown; cumulative-flow diagram for bottlenecks | Whether scope, throughput, or work-in-progress is the constraint |
| Is a predictive project on schedule or budget? | EVM table and trend chart | Forecast completion and decide on corrective action |
| Why did a failure or variance occur? | 5 Whys; fishbone diagram; Pareto chart for recurring patterns | Root causes and the highest-leverage improvement |
| Which option/change should be approved? | Change-impact assessment + decision log | Benefit, impact, risk, approval, implementation/rollback |
| Are stakeholders aligned and informed? | Stakeholder map + communications plan + concise status update | Audience, channel, decision, and next update |
| Is delivery ready to become a service? | Service-readiness / handover checklist | Whether support ownership and controls are workable |

## Progress and schedule problems

### Use a milestone plan first

Use for any project. Track major deliverables, planned versus forecast dates, owner, dependency, status, and recovery action. It gives leaders a readable view before deeper analysis.

| Milestone | Baseline date | Forecast date | Variance | Dependency/blocker | Recovery action | Owner |
|---|---:|---:|---:|---|---|---|

### Add a dependency map or critical-path analysis when the finish date is at risk

Use when tasks have linked predecessors and you have estimated durations. Analyse the chain with zero/low float before asking people to “work harder.” A delay off the critical path may consume float without moving the end date; a critical-path delay requires a recovery decision.

Possible actions: remove a blocker, resequence compatible work, add qualified capacity, reduce or defer approved scope, fast-track where risk is acceptable, or request a formally approved date change.

### Use agile flow charts only for iterative delivery

- **Burnup:** show delivered work against total scope; best when scope changes must stay visible.
- **Burndown:** show remaining work toward a sprint/release goal; best for short, stable timeboxes.
- **Cumulative-flow diagram:** show work by state over time; best for identifying a queue/bottleneck and excessive work in progress.
- **Velocity/throughput trend:** plan a near-term forecast from comparable completed iterations, not as an individual performance target.

Do not compare velocity across different teams or forecast a long-term date from one unrepresentative iteration.

### Use EVM only when its baseline is trustworthy

EVM is useful in predictive or governed hybrid work when scope/work packages, schedule baseline, budget baseline, and actual performance/cost data exist.

| Measure | Meaning | Management use |
|---|---|---|
| PV (planned value) | Budgeted work planned by the date | Baseline expectation |
| EV (earned value) | Budgeted value of accepted completed work | Progress measure |
| AC (actual cost) | Cost actually incurred | Actual spend |
| SPI = EV / PV | Schedule efficiency | Below 1: less work completed than planned |
| CPI = EV / AC | Cost efficiency | Below 1: cost is exceeding earned value |
| EAC | Forecast total cost at completion | Funding/forecast decision |

EVM indicates a performance variance; it does not explain its cause. Pair it with dependency review and root-cause analysis. Never manufacture precision when EV or AC is unavailable.

## Analysis tools: match the tool to the failure mode

| Situation | Tool | Result |
|---|---|---|
| One recent issue/variance | 5 Whys | A testable causal chain and immediate corrective action |
| Several possible causes | Fishbone (people, process, technology, materials/data, environment, measurement) | Structured causes to investigate |
| Many repeated defects/incidents | Pareto chart | Which categories create most impact/frequency |
| Process is unstable over time | Run chart/control chart | Signal versus normal variation; whether to investigate a special cause |
| Competing alternatives | Decision matrix with agreed criteria/weights | Transparent recommendation, not automatic approval |

For a live incident, restore service and communicate first. Root-cause tools belong to the follow-up problem review unless immediate safety or compliance demands otherwise.

## Minimum control set by delivery approach

| Context | Minimum control set |
|---|---|
| Small predictive project | Milestone plan, WBS/work packages, RAID log, risk register, change/decision log, customer update |
| Agile product delivery | Prioritized backlog, acceptance criteria, iteration goal, burnup or board/flow view, impediment log, retrospective actions |
| Hybrid project | Milestone and baseline controls for governed commitments; backlog/flow measures for iterative scope; one shared RAID/change log |
| Live service | Incident/request/change records, service level/status trends, knowledge/runbooks, problem and improvement backlog |

## Recommended output format

When advising the user, give:

1. the decision they need to make;
2. the one or two recommended tools and why;
3. the minimum fields/data to collect;
4. what the evidence suggests or cannot yet prove;
5. the next action, owner, and approval/escalation point.

Do not overwhelm a small project with all tools. Begin with a milestone view plus RAID/action/decision records, then add analysis only when a meaningful variance or decision arises.
