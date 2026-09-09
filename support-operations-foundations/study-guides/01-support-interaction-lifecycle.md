# 01 — Support Interaction Lifecycle

## Purpose

A support interaction is more than fixing a technical problem.

A technician must:

1. receive the user's request;
2. understand what the user is actually reporting;
3. collect enough information to define the issue;
4. document relevant information;
5. investigate or take action;
6. communicate progress;
7. resolve the issue or escalate it;
8. validate the result;
9. document the outcome;
10. close the interaction appropriately.

This guide introduces the complete support lifecycle before later guides examine each stage in greater depth.

---

## 1. Support Is a Process

A common beginner mistake is to think of support as:

> User reports problem → Technician fixes problem

Real support is usually more structured.

A better model is:

```text
User Request
    ↓
Acknowledge
    ↓
Clarify
    ↓
Define the Issue
    ↓
Document
    ↓
Investigate / Take Action
    ↓
Communicate Progress
    ↓
Resolve or Escalate
    ↓
Validate
    ↓
Document Resolution
    ↓
Close
```

The exact order may change depending on the situation.

For example:

- a critical outage may require immediate action before complete documentation;
- a simple password reset may be resolved very quickly;
- a complicated incident may move several times between investigation, communication and escalation.

The important principle is that support should be **structured rather than improvised**.

---

## 2. Stage 1 — Receive the Request

Every support case begins with some type of request.

The user may contact support through:

- chat;
- email;
- ticket;
- phone;
- video call;
- remote-support session;
- in-person conversation.

The first message may be detailed:

> My Canon printer appears Offline in Windows. It was working yesterday, but I cannot print from the reception PC this morning.

Or extremely vague:

> Printer doesn't work.

Both are support requests.

However, they do not contain the same amount of usable information.

The technician's first task is therefore not necessarily to solve the problem.

The first task is to determine:

> **What is the user actually reporting?**

---

## 3. Stage 2 — Acknowledge the Request

Acknowledgement confirms that the request has been received and understood.

For example:

> I understand that you are currently unable to print from the reception computer.

Acknowledgement is useful because it establishes shared understanding.

It does **not** mean that the technician already knows the cause.

It also does not require promising an immediate solution.

### Weak

> OK.

### Risky

> Don't worry. I'll fix it immediately.

### Better

> I understand that you are unable to print. I'll first check what is happening and determine the next step.

The last response acknowledges the issue without making a promise before diagnosis.

---

## 4. Stage 3 — Clarify

Many user reports are incomplete.

Example:

> Internet is not working.

This does not tell us:

- which device is affected;
- whether Wi-Fi or Ethernet is being used;
- whether the device has network connectivity;
- whether only websites are unavailable;
- whether DNS is failing;
- whether other users are affected;
- when the issue started;
- whether anything changed beforehand.

A support technician should therefore ask questions that reduce uncertainty.

For example:

> Is the issue happening only on your computer or are other users affected as well?

> Are you connected through Wi-Fi or Ethernet?

> What happens when you try to open a website?

> Did the connection work normally earlier today?

Clarification is not random questioning.

Each question should help define the problem more precisely.

---

## 5. Do Not Confuse a Symptom With a Diagnosis

This is one of the most important support habits.

If a user says:

> Outlook isn't receiving emails.

That is a **reported symptom**.

It does not automatically mean:

> Outlook synchronization is broken.

Possible causes could include:

- network connectivity;
- authentication;
- account configuration;
- mail server availability;
- mailbox rules;
- Outlook state;
- user configuration;
- a wider service issue.

Until there is evidence, the cause remains unknown.

A technician should therefore separate:

```text
Reported symptom:
User reports that Outlook is not receiving new messages.
```

from:

```text
Diagnosis:
Not yet determined.
```

This prevents premature conclusions.

---

## 6. Stage 4 — Define the Issue

After clarification, the technician should be able to describe the issue more precisely.

Instead of:

> Printer broken.

A useful description might be:

```text
User:
Reception employee

Device:
Canon USB printer connected to reception workstation

Issue:
User cannot print.

Observed behavior:
Windows reports the printer as Offline.

Scope:
One workstation currently confirmed affected.

Started:
This morning.

Previous action:
Printer restarted by user with no change.
```

Notice that this does not yet claim to know the cause.

It defines what is currently known.

---

## 7. Stage 5 — Document

Support information should not exist only in the technician's memory.

Depending on the environment, documentation may exist in:

- a ticketing system;
- service desk software;
- internal notes;
- work-order software;
- incident records;
- maintenance records.

Useful documentation may include:

```text
Issue
Affected user
Affected device/service
Impact
Symptoms
Evidence
Actions performed
Results
Status
Next action
Owner
Resolution
```

Not every case requires every field.

The objective is to preserve enough information that the case can be understood and continued.

---

## 8. Stage 6 — Investigate

Only after the problem is sufficiently understood should systematic troubleshooting begin.

A useful troubleshooting pattern is:

```text
Evidence
    ↓
Possible Cause
    ↓
Test
    ↓
Result
    ↓
Interpretation
    ↓
Next Action
```

### Example

```text
Evidence:
Printer appears Offline in Windows.

Possible cause:
Windows may not be detecting the USB printer.

Test:
Check Windows USB device detection.

Result:
USB device appears with a device-descriptor error.

Interpretation:
The workstation is not communicating correctly with the USB device.

Next action:
Test the USB cable or port and verify device detection again.
```

The technician is now moving from observation toward diagnosis.

---

## 9. Actions and Results Are Different

Support notes should distinguish what was done from what happened afterward.

### Weak documentation

> Checked network and DNS.

### Better documentation

```text
Action:
Ran ipconfig /all.

Result:
Workstation was using a public DNS server instead of the internal DNS server.

Action:
Changed DNS configuration to the internal DNS server.

Result:
Workstation successfully resolved the domain controller.
```

This distinction is extremely important.

A support record should allow another technician to understand:

> **What did you do, and what did that action prove?**

---

## 10. Stage 7 — Communicate Progress

The technician should not disappear while investigating.

Users need enough information to understand what is happening.

### Weak

> We're working on it.

### Better

> The computer is connected to the network, but it is currently unable to locate the company login server. I'm checking the DNS configuration now and will update you after that test.

A useful status update can contain:

```text
Current situation
+
What has been checked
+
What is happening now
+
What happens next
```

Good communication reduces uncertainty even when the problem has not yet been resolved.

---

## 11. Stage 8 — Resolve or Escalate

Investigation eventually leads to one of several outcomes.

### Resolution

The technician identifies and corrects the issue.

### Further Investigation

Additional evidence or testing is required.

### Escalation

The issue requires another technician, team, vendor or authority.

Possible reasons for escalation include:

- insufficient permissions;
- problem outside the technician's scope;
- security requirement;
- specialist knowledge required;
- documented escalation rule;
- repeated troubleshooting failure;
- service or infrastructure controlled by another team.

Escalation is not failure.

A good escalation transfers the case **with useful context**.

---

## 12. Escalation Should Preserve Work Already Done

### Poor escalation

> Doesn't work. Please check.

### Useful escalation

```text
Issue:
User cannot authenticate to application.

Impact:
User is unable to access the system.

Evidence:
Authentication error reproduced.

Actions completed:
- Confirmed network connectivity
- Confirmed account username
- Cleared application cache
- Reproduced issue
- Captured error log

Result:
Authentication error persists.

Reason for escalation:
Issue continues after documented first-line troubleshooting.

Requested next action:
Review authentication logs.

Current user expectation:
User has been informed that the issue is being transferred for further investigation.
```

A strong escalation prevents the next technician from starting from zero.

---

## 13. Stage 9 — Validate

Performing a technical action does not automatically mean the issue is resolved.

For example:

> Technician reinstalls the printer driver.

That is an **action**.

Resolution still needs to be validated.

```text
Test:
Printed Windows test page.

Result:
Successful.

User validation:
User successfully printed the required document.
```

The important question is:

> **Does the original problem still exist?**

---

## 14. Technical Success vs User Success

These are related but not identical.

Suppose:

```text
Ping to server: successful
DNS resolution: successful
Authentication test: successful
```

Technically, the infrastructure may look healthy.

But if the user still cannot complete their task, the support case may not actually be resolved.

Whenever practical, validation should return to the original user goal.

### Original issue

> User cannot print customer invoice.

### Final validation

> User successfully prints customer invoice.

That is stronger than:

> Printer responds to ping.

---

## 15. Stage 10 — Document the Resolution

The final ticket should explain what actually resolved the issue.

### Weak

> Fixed.

### Better

```text
Identified cause:
Workstation was configured with an incorrect DNS server.

Resolution:
DNS configuration changed to the internal DNS server.

Validation:
Domain controller resolved successfully and user logged into the workstation.

User confirmation:
User confirmed successful login.

Status:
Resolved.
```

Resolution documentation helps with:

- future repeated incidents;
- knowledge transfer;
- trend analysis;
- troubleshooting efficiency;
- accountability.

---

## 16. Stage 11 — Close

Before closure, consider:

- Was the original issue resolved?
- Was the result tested?
- Has the user confirmed success when appropriate?
- Are the important actions documented?
- Is follow-up still required?
- Is another team responsible for anything?
- Are there unresolved risks or questions?

Only then should the case be considered complete.

---

## 17. The Support Lifecycle Is a Loop

Troubleshooting rarely follows a perfect straight line.

A more realistic model is:

```text
                    ┌──────────────────────────┐
                    │                          │
                    ▼                          │
Request → Clarify → Investigate → Test → Result
                    ▲                   │
                    │                   │
                    │             Not Resolved
                    │                   │
                    └──── More Evidence ┘

                              ↓
                           Resolved
                              ↓
                           Validate
                              ↓
                           Document
                              ↓
                            Close
```

You may repeatedly:

- ask new questions;
- collect more evidence;
- perform another test;
- consult documentation;
- communicate another update;
- escalate;
- receive the case back.

This is normal.

The objective is not to follow a rigid script.

The objective is to maintain a **structured support process**.

---

## 18. A Useful Mental Model

When a user reports a problem, think through six questions.

### What do I know?

Facts and evidence.

### What do I not know?

Missing information.

### What am I assuming?

Possible assumptions that still need verification.

### What can I test?

The next useful diagnostic action.

### What did the test prove?

The result and its interpretation.

### What happens next?

The next action, escalation or resolution.

This prevents random troubleshooting.

---

## 19. Full Example — From Report to Closure

### Initial Report

> I can't print.

### Clarification

The technician determines:

```text
User:
Front desk

Printer:
Canon USB printer

Computer:
Front-desk workstation

Symptom:
Windows shows printer as Offline.

Scope:
Only one workstation currently known to be affected.

Started:
This morning.

Previous action:
Printer restarted.
```

### Investigation

```text
Action:
Checked Windows printer status.

Result:
Printer still Offline.

Action:
Checked USB device detection.

Result:
USB device detection error observed.

Action:
Moved printer to another USB port.

Result:
Device detected successfully.

Action:
Printed test page.

Result:
Successful.
```

### Validation

```text
Test:
User asked to print normal customer document.

Result:
Successful.
```

### Resolution

```text
Issue:
Printer unavailable because workstation was not detecting the USB device correctly.

Resolution:
Printer reconnected through a working USB port.

Validation:
Test page and user document printed successfully.

Status:
Resolved.
```

---

## 20. Key Principles

Remember:

1. **Understand before assuming.**
2. **Separate symptoms from diagnosis.**
3. **Ask questions that reduce uncertainty.**
4. **Document facts, actions and results.**
5. **Troubleshoot systematically.**
6. **Keep the user informed.**
7. **Escalate with context.**
8. **Validate the original user problem.**
9. **Document the resolution.**
10. **Close only when the support process is complete.**

---

## Self-Check

Before moving to the exercises, you should be able to explain:

- Why is a user report not necessarily a diagnosis?
- What is the difference between clarification and troubleshooting?
- What is the difference between an action and a result?
- Why should a status update contain more than “working on it”?
- When might escalation be appropriate?
- Why is performing a fix not the same as validating a resolution?
- Why does the user's original goal matter during validation?
- What should be documented before closure?

If any of these are unclear, review the relevant section before continuing.

---

## Next Step

Complete:

`exercises/01-support-interaction-exercises.md`

before moving to:

`study-guides/02-request-intake-and-clarification.md`
