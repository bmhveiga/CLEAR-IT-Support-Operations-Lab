# 02 — Request Intake and Clarification

## Purpose

Before troubleshooting a problem, a support technician needs to understand what the problem actually is.

Users rarely describe technical issues in the same way a technician would document them.

A user may say:

> The printer isn't working.

> I can't log in.

> The internet is bad.

> Outlook is broken.

> My computer is slow.

These statements are useful because they tell us that the user needs support.

However, they usually do **not** contain enough information to begin structured troubleshooting.

The purpose of request intake is to transform an initial user report into a clear and actionable description of the problem.

A useful mental model is:

```text
User Report
    ↓
Clarification
    ↓
Relevant Facts
    ↓
Scope + Impact + Evidence
    ↓
Defined Support Issue
    ↓
Troubleshooting
```

This guide focuses on everything that happens **before troubleshooting begins**.

---

## 1. What Is Request Intake?

Request intake is the process of receiving a support request and collecting the information needed to understand it.

The technician is trying to answer questions such as:

- Who is affected?
- What is affected?
- What exactly is happening?
- What should happen instead?
- When did it start?
- How many users or devices are affected?
- What evidence is available?
- What has already been tried?
- What changed before the issue started?
- How much is the problem affecting the user's work?

The objective is not to interrogate the user.

The objective is to reduce uncertainty.

---

## 2. The User Describes Experience — The Technician Defines the Issue

Users normally describe what they experience.

For example:

> My computer has no internet.

That statement reflects the user's experience.

But technically, several different situations could produce the same experience:

- Wi-Fi disconnected;
- Ethernet cable disconnected;
- no IP address;
- incorrect gateway;
- DNS failure;
- browser problem;
- authentication portal problem;
- router outage;
- ISP outage;
- only one website unavailable.

The technician should therefore treat the initial report as:

> **the starting point of the investigation**

rather than:

> **the confirmed technical diagnosis**

---

## 3. Reported Symptom vs Confirmed Fact vs Diagnosis

These three concepts should remain separate.

### Reported Symptom

What the user says they are experiencing.

```text
User reports that the internet is not working.
```

### Confirmed Fact

Something the technician has verified.

```text
The workstation has an IPv4 address but cannot resolve domain names.
```

### Diagnosis

The identified cause of the issue.

```text
The workstation is configured with an incorrect DNS server.
```

These may occur at very different stages of the support lifecycle.

Do not turn:

```text
User says:
"The internet doesn't work."
```

into:

```text
Diagnosis:
Router failure.
```

without evidence.

---

## 4. Clarification Is About Reducing Uncertainty

A weak clarification question is:

> Can you explain?

It may help, but it gives the user very little direction.

A stronger question targets specific missing information.

For example:

> What happens when you try to open a website?

Or:

> Are other users having the same problem, or is it only happening on your computer?

Or:

> Do you see an error message when you try to log in?

Each question removes uncertainty from the case.

A good clarification question should have a reason.

Before asking something, consider:

> **What will this answer help me understand?**

---

## 5. The Core Intake Categories

A useful IT support intake can be organized into several categories.

```text
WHO
WHAT
WHERE
WHEN
SCOPE
IMPACT
EVIDENCE
CHANGES
REPRODUCIBILITY
PREVIOUS ACTIONS
```

You will not need every category for every issue.

The categories help you remember what information may be missing.

---

# 6. WHO — Who Is Affected?

Identify the affected user or group.

Questions may include:

> Is this happening only to you?

> Are other users experiencing the same issue?

> Which user account is affected?

Why this matters:

One affected user and an entire department experiencing the same symptom may indicate very different support situations.

Compare:

```text
One user cannot log in.
```

with:

```text
All users in the Finance department cannot log in.
```

The symptom may look similar.

The scope is completely different.

---

# 7. WHAT — What Is Actually Failing?

Avoid vague descriptions such as:

> Computer doesn't work.

Clarify the actual behavior.

Possible questions:

> Does the computer power on?

> Does Windows start?

> Are you able to log in?

> Does the application open?

> What happens when you try to print?

The phrase:

> Computer doesn't work.

could mean:

```text
No power
No display
Windows does not boot
Login fails
Application does not open
Network unavailable
Computer is extremely slow
```

These are different support problems.

---

## 8. Expected Behavior vs Actual Behavior

One of the most useful ways to define an issue is:

```text
Expected:
What should happen?

Actual:
What happens instead?
```

Example:

```text
Expected:
User enters domain credentials and Windows opens the desktop.

Actual:
Windows displays "The user name or password is incorrect."
```

Another example:

```text
Expected:
Document should print on reception printer.

Actual:
Print job remains in queue and Windows shows printer as Offline.
```

This comparison makes the problem much clearer.

---

# 9. WHERE — Identify the Affected Asset or Service

Determine exactly what is involved.

This might be:

- workstation;
- laptop;
- printer;
- account;
- application;
- server;
- website;
- network;
- shared folder;
- email service;
- phone;
- CCTV system;
- POS system.

Instead of:

> Printer is not working.

identify:

```text
Printer:
Canon LBP6030

Workstation:
Front Desk PC

Connection:
USB
```

Specific assets make documentation and troubleshooting easier.

---

# 10. WHEN — Establish the Timeline

Time information can provide important context.

Ask:

> When did this start?

> Was it working before?

> When was the last time it worked normally?

> Did it stop suddenly or gradually become worse?

Compare:

```text
Printer has never worked on this PC.
```

with:

```text
Printer worked normally yesterday and became Offline this morning.
```

The second statement suggests that something may have changed.

---

# 11. SCOPE — How Large Is the Problem?

Scope identifies how much of the environment is affected.

A simple scope progression is:

```text
One user
↓
One device
↓
Several users
↓
One department/location
↓
Multiple departments
↓
Entire organization/service
```

Example:

User says:

> The internet is down.

Before treating it as an organization-wide outage, determine scope.

Ask:

> Is this happening on other computers too?

> Are both Wi-Fi and Ethernet affected?

> Are users in another part of the office having the same issue?

You may discover:

```text
Only one laptop is affected.
```

That completely changes the investigation.

---

## 12. Scope Is One of the Fastest Ways to Narrow a Problem

Consider:

```text
User cannot print.
```

### Scenario A

Only one workstation cannot print.

Possible investigation may focus on:

- workstation;
- driver;
- port;
- print queue;
- local connectivity.

### Scenario B

Nobody can print to the printer.

The investigation may shift toward:

- printer availability;
- network connection;
- printer hardware;
- shared print service.

### Scenario C

One user cannot print from any workstation.

The investigation may shift toward:

- account;
- permissions;
- application;
- user-specific configuration.

Same general complaint.

Very different scope.

---

# 13. IMPACT — What Is the User Unable to Do?

Impact describes the effect of the issue on work.

Instead of recording only:

> Printer offline.

consider:

> Reception employee cannot print customer invoices.

The second description tells us why the issue matters.

Questions may include:

> Is this preventing you from working?

> Can you continue using another system or device?

> Is there another printer available?

> Which task are you currently unable to complete?

Impact might range from:

```text
Minor inconvenience
```

to:

```text
One user unable to perform an important task
```

to:

```text
Multiple users unable to perform business-critical work
```

Understanding impact helps the support team decide how urgently the issue should be handled.

---

# 14. Impact and Technical Severity Are Not Always the Same

A technically simple issue can have high business impact.

Example:

```text
Technical issue:
Printer queue stopped.

Business impact:
Front desk cannot print required customer documents.
```

A technically complex issue may have low immediate impact.

Example:

```text
Technical issue:
Secondary monitoring dashboard unavailable.

Business impact:
No users blocked; primary monitoring remains operational.
```

Support work should consider both the technical problem and its effect on the user or business.

---

# 15. EVIDENCE — What Can Be Observed?

Evidence is more useful than interpretation.

Useful evidence may include:

- exact error message;
- error code;
- screenshot;
- log entry;
- printer status;
- Windows status;
- LED behavior;
- command output;
- timestamp;
- reproducible behavior.

Compare:

### Weak

> Login seems broken.

### Better

```text
After entering credentials, Windows displays:
"The user name or password is incorrect."
```

Evidence gives the investigation something concrete to work with.

---

## 16. Ask for Exact Error Messages

Users may paraphrase errors.

For example:

> It says something about the password.

That may not be enough.

Ask:

> Could you tell me the exact message shown on the screen?

Or:

> Could you send a screenshot of the error?

The exact wording may reveal important information.

For example:

```text
"Password incorrect"
```

is different from:

```text
"Domain is unavailable"
```

even though the user might describe both as:

> I can't log in.

---

# 17. Screenshots Are Evidence — But Review Them Carefully

Screenshots can be extremely useful because they preserve:

- exact messages;
- interface state;
- timestamps;
- status indicators;
- configuration information.

However, screenshots may also expose:

- personal information;
- email addresses;
- usernames;
- customer data;
- network information;
- sensitive internal information.

Do not request or share more information than is necessary for the support case.

Never ask the user to send their password.

---

# 18. CHANGES — What Changed Before the Problem Started?

This is one of the highest-value questions in troubleshooting.

Ask:

> Did anything change before the issue started?

Possible changes include:

- software installation;
- Windows update;
- password change;
- new network connection;
- device relocation;
- cable replacement;
- driver update;
- configuration change;
- new hardware;
- account change.

Example:

User:

> I can't log in anymore.

Additional information:

> My password was changed yesterday.

That change may become highly relevant to the investigation.

Do not assume the change caused the issue.

Treat it as evidence.

---

# 19. Correlation Is Not Automatically Causation

Suppose:

```text
Windows updated last night.
Printer stopped working this morning.
```

It is reasonable to record the update as a recent change.

It is **not** yet reasonable to state:

```text
Cause:
Windows Update broke printer.
```

You still need evidence.

Write:

```text
Recent change:
Windows updates installed the previous evening.
```

Then investigate whether that change is actually related.

---

# 20. REPRODUCIBILITY — Can the Problem Be Repeated?

Ask:

> Does this happen every time?

> Can you show me what happens?

> Does it happen with every document or only this one?

> Does it happen in another browser?

Reproducibility helps determine whether the issue is:

```text
Consistent
Intermittent
Situation-specific
User-specific
Device-specific
Application-specific
```

Example:

```text
Printing fails with every document.
```

is different from:

```text
Only one PDF fails to print.
```

---

# 21. PREVIOUS ACTIONS — What Has Already Been Tried?

Before repeating troubleshooting unnecessarily, ask what the user or another technician has already done.

For example:

> Have you already restarted the application or computer?

> Has anyone else worked on this issue?

> What troubleshooting has already been attempted?

Document previous actions.

Example:

```text
Previous actions:
- User restarted printer
- USB cable disconnected and reconnected
- Issue persists
```

This prevents duplicated effort.

---

# 22. Do Not Let the User's Diagnosis Replace Your Intake

Users sometimes provide their own diagnosis.

Example:

> The router is broken.

Treat that statement carefully.

Ask:

> What are you seeing that makes you think the router is the problem?

You may discover:

```text
Only one website is unavailable.
```

The user's diagnosis may be correct.

But it still needs verification.

A useful ticket might say:

```text
User reports internet connectivity problem and suspects router issue.

Confirmed cause:
Not yet determined.
```

---

# 23. Avoid Leading Questions

A leading question pushes the user toward a particular answer.

Example:

> The problem started after the Windows update, right?

This encourages confirmation of your hypothesis.

Better:

> Do you remember whether anything changed on the computer before the issue started?

Or:

> When did the problem first appear?

Good intake gathers information rather than trying to prove the technician's first idea.

---

# 24. Avoid Asking Too Many Questions at Once

Consider this message:

> Which PC is it, when did it start, what's the error, are others affected, did you restart, is it Wi-Fi, did Windows update, what browser are you using, and can you send a screenshot?

Technically, these may all be useful questions.

But for a user, this may feel overwhelming.

In interactive support, ask questions in logical groups.

For example:

> What happens when you try to connect?

Wait for answer.

Then:

> Is this happening only on your computer, or are other users affected?

Then:

> Thanks. Are you connected through Wi-Fi or Ethernet?

Support should feel like a guided investigation.

---

# 25. Broad Questions vs Targeted Questions

Both have a place.

### Broad Question

> What happens when you try to print?

Useful early because it lets the user describe the behavior.

### Targeted Question

> Does Windows show the printer as Offline?

Useful after you have narrowed the problem.

A useful pattern is:

```text
Broad
↓
Observe answer
↓
Targeted
↓
Narrow issue
↓
Targeted test
```

Avoid beginning with twenty technical yes/no questions when you do not yet understand the basic problem.

---

# 26. Ask One Question for a Reason

Every useful question should connect to something you are trying to learn.

Example:

### Question

> Can other users print to the same printer?

### Why ask it?

To determine scope.

---

### Question

> When did the issue start?

### Why ask it?

To establish timeline and possible changes.

---

### Question

> What exact error message appears?

### Why ask it?

To collect evidence.

---

### Question

> Does it happen every time?

### Why ask it?

To determine reproducibility.

---

### Question

> Can you use another printer?

### Why ask it?

To understand impact and possible workaround.

---

# 27. From Vague Request to Defined Issue

Initial report:

> Printer doesn't work.

After clarification:

```text
User:
Reception employee

Workstation:
Front Desk PC

Printer:
Canon USB printer

Expected behavior:
Document should print normally.

Actual behavior:
Windows reports printer as Offline and document remains in print queue.

Started:
This morning.

Previous state:
Printer worked yesterday.

Scope:
Only Front Desk PC currently confirmed affected.

Impact:
User cannot print customer documents.

Evidence:
Windows printer status shows Offline.

Previous actions:
User restarted printer and reconnected USB cable.

Recent changes:
None currently known.

Diagnosis:
Not yet determined.
```

Now we have an actionable support issue.

Notice what we **do not** have:

```text
Cause:
USB driver failure
```

because that has not yet been established.

---

# 28. Example — Login Problem

Initial report:

> I can't log in.

Possible clarification process:

### Step 1 — Identify where

> Are you trying to log into Windows or into an application?

User:

> Windows.

### Step 2 — Collect evidence

> What message appears after you enter your credentials?

User:

> It says the username or password is incorrect.

### Step 3 — Determine scope

> Are you able to log into another computer with the same account?

User:

> I haven't tried.

### Step 4 — Determine timing

> Was this login working previously?

User:

> Yes, yesterday.

### Step 5 — Identify changes

> Did your password or account change recently?

User:

> My password was reset yesterday.

We now know much more than:

> I can't log in.

But we still have not diagnosed the cause.

---

# 29. Example — Slow Internet

Initial report:

> Internet is very slow.

Clarification may investigate:

```text
Who:
One user or several?

Device:
Laptop, desktop, phone?

Connection:
Wi-Fi or Ethernet?

Behavior:
All websites slow or one application?

Time:
Always slow or started recently?

Location:
One room or everywhere?

Scope:
One device or multiple devices?

Evidence:
Speed test, latency, packet loss, network status.

Changes:
New access point? Network change? Device update?
```

Again, the objective is not to immediately blame:

```text
Wi-Fi
ISP
router
DNS
```

The objective is first to understand the pattern.

---

# 30. Example — Outlook Not Receiving Emails

Initial report:

> Outlook isn't receiving emails.

Useful intake questions might include:

> When was the last message you received?

> Can you send email successfully?

> Does Outlook show any connection or synchronization error?

> Can you access the mailbox through webmail?

> Are other users experiencing the same issue?

> Are you expecting one specific message, or are no new messages arriving at all?

That last question is particularly important.

The problem may actually be:

```text
One expected email has not arrived.
```

rather than:

```text
Outlook is not receiving any email.
```

Those are not the same issue.

---

# 31. Clarification Can Change the Entire Problem

Initial request:

> Outlook isn't receiving emails.

After clarification:

```text
Outlook is receiving normal email.

User is waiting for one verification-code email from a specific service.

Other messages are arriving normally.
```

The original problem has now changed from:

```text
Possible Outlook synchronization issue
```

to:

```text
Specific expected message not received
```

This is why good intake matters.

You may eliminate entire troubleshooting paths before touching the computer.

---

# 32. Intake Should Be Proportional to the Issue

Not every issue needs a long interview.

Example:

User:

> I forgot my password and need it reset.

If identity and reset procedures are clear, the request may be handled quickly.

Another example:

> Nobody in the office can access the network.

That may require immediate scope confirmation and rapid response.

The purpose of the intake framework is not to create bureaucracy.

It is to collect **enough information for the situation**.

---

# 33. Urgent Situations May Change the Order

Suppose several users report:

> The company network is completely unavailable.

You may need to quickly confirm:

```text
Multiple users affected?
Multiple devices?
Wi-Fi and Ethernet?
Critical services unavailable?
```

and begin incident response immediately.

You do not need to complete a perfect ticket before taking any action.

But documentation should still catch up as the incident progresses.

Structured support does not mean rigid support.

---

# 34. A Compact Intake Framework

For everyday support, remember:

```text
USER
Who is affected?

ASSET
What device, account, application or service?

SYMPTOM
What exactly happens?

EXPECTED
What should happen instead?

TIME
When did it start?

SCOPE
Who or what else is affected?

IMPACT
What work cannot be completed?

EVIDENCE
What error, screenshot or observable behavior exists?

CHANGE
What changed before it started?

REPRODUCIBILITY
Does it happen consistently?

PREVIOUS ACTIONS
What has already been tried?
```

You do not have to ask these in this exact order.

Use them as a checklist for missing information.

---

# 35. The Minimum Actionable Ticket

A ticket does not have to contain the final diagnosis before investigation begins.

But it should contain enough information that another technician can understand the starting situation.

A useful minimum might be:

```text
User:
Affected asset/service:

Reported issue:

Observed behavior:

Started:

Scope:

Impact:

Evidence:

Previous actions:

Current status:

Next step:
```

Example:

```text
User:
Reception employee

Affected asset:
Canon USB printer on Front Desk PC

Reported issue:
User unable to print.

Observed behavior:
Windows shows printer as Offline.

Started:
This morning.

Scope:
One workstation currently confirmed affected.

Impact:
User cannot print customer documents.

Evidence:
Printer status shows Offline.

Previous actions:
Printer restarted and USB cable reconnected.

Current status:
Open — troubleshooting not yet started.

Next step:
Verify USB detection and printer queue.
```

---

# 36. What Not to Invent

If the user has not told you something and you have not verified it, do not silently add it.

For example:

Known:

```text
User cannot print.
Printer shows Offline.
```

Do not invent:

```text
Cause:
Driver corrupted.

Priority:
Critical.

Started:
08:00.

Other users:
Unaffected.
```

Unknown information should remain unknown until confirmed.

You can document:

```text
Scope:
Not yet confirmed.
```

That is better than guessing.

---

# 37. Facts, Unknowns and Assumptions

A useful technique during intake is to divide information into three groups.

```text
FACTS
- User cannot print
- Windows shows printer Offline
- Printer was restarted

UNKNOWNS
- Whether other PCs can print
- Whether Windows detects USB device
- Whether print queue contains stuck jobs

ASSUMPTIONS
- Possible USB connection issue
- Possible driver/port issue
```

This makes your reasoning much cleaner.

Facts can be documented confidently.

Unknowns become clarification questions or tests.

Assumptions become hypotheses — not conclusions.

---

# 38. Stop Intake When You Have Enough to Act

Clarification can become excessive.

At some point you should have enough information to begin troubleshooting.

For example:

```text
User:
Front desk

Asset:
USB printer

Symptom:
Offline in Windows

Scope:
One PC

Impact:
Cannot print invoices

Evidence:
Offline status

Previous action:
Restart unsuccessful
```

At this point, asking another fifteen questions may not be useful.

The next appropriate step is probably investigation.

Good support balances:

```text
Enough information
+
Efficient action
```

---

# 39. Intake Quality Check

Before moving into troubleshooting, ask yourself:

### Understanding

Can I clearly describe what the user is experiencing?

### Asset

Do I know which device, account or service is involved?

### Symptom

Do I know the actual observed behavior?

### Scope

Do I know whether one or multiple users/devices are affected?

### Impact

Do I understand what the user cannot do?

### Evidence

Do I have an error message, status or other useful evidence where available?

### Timeline

Do I know when the issue started or whether it worked previously?

### Changes

Have relevant recent changes been identified?

### Previous Actions

Do I know what has already been attempted?

### Assumptions

Have I avoided presenting guesses as facts?

If enough of these are known to begin a meaningful investigation, intake has done its job.

---

# 40. Full Intake Example

## User Report

> The internet isn't working on my computer.

## Technician Clarification

### Question 1

> What happens when you try to open a website?

### Answer

> The browser says the page can't be reached.

### Question 2

> Is this happening only on your computer, or are other users affected?

### Answer

> Everyone else seems to have internet.

### Question 3

> Are you connected through Wi-Fi or Ethernet?

### Answer

> Ethernet.

### Question 4

> Was it working earlier today?

### Answer

> Yes. It stopped around lunchtime.

### Question 5

> Did anything change on the computer or network connection before it stopped?

### Answer

> I moved the computer to another desk after lunch.

### Question 6

> Do you see a network icon showing disconnected, or does Windows show that you are connected?

### Answer

> It says no network.

---

## Defined Intake Record

```text
User:
Single office user

Affected device:
Desktop workstation

Reported issue:
User unable to access internet.

Expected behavior:
Workstation should connect to office LAN and internet through Ethernet.

Actual behavior:
Browser cannot load websites and Windows reports no network connection.

Started:
Around lunchtime.

Previous state:
Connection worked earlier today.

Scope:
One workstation currently affected.
Other users appear unaffected.

Impact:
User cannot access internet-dependent work resources.

Connection:
Ethernet.

Recent change:
Workstation was moved to another desk shortly before issue began.

Evidence:
Windows reports no network connection.

Previous actions:
None reported.

Diagnosis:
Not yet determined.

Next step:
Verify physical Ethernet connection and network link at the new desk.
```

Notice how much clearer the case has become.

We have not yet fixed anything.

But we now know **where to begin**.

---

# 41. Key Principles

Remember:

1. **The user's first message is a starting point, not a diagnosis.**
2. **Clarification should reduce uncertainty.**
3. **Ask questions for a reason.**
4. **Separate reported symptoms, confirmed facts and diagnoses.**
5. **Identify the affected user, asset and service.**
6. **Compare expected behavior with actual behavior.**
7. **Determine scope before assuming an outage is widespread.**
8. **Understand the effect on the user's work.**
9. **Collect evidence instead of relying only on interpretation.**
10. **Ask about recent changes without assuming they caused the issue.**
11. **Determine whether the problem is reproducible.**
12. **Document previous troubleshooting.**
13. **Do not invent missing information.**
14. **Stop asking questions when you have enough information to act.**

---

## Self-Check

Before moving to the exercises, you should be able to explain:

- What is the purpose of request intake?
- Why should the user's diagnosis not automatically become the ticket diagnosis?
- What is the difference between a reported symptom, confirmed fact and diagnosis?
- Why is expected behavior useful?
- Why is scope important?
- What does impact tell the technician?
- Why should exact error messages be collected?
- Why are recent changes useful without necessarily proving cause?
- What is reproducibility?
- Why should previous troubleshooting be recorded?
- What is wrong with leading questions?
- When should clarification stop and troubleshooting begin?
- Why is `Unknown` better than invented information?

If any of these are unclear, review the relevant section before continuing.

---

## Quick Reference — Intake Checklist

```text
[ ] Who is affected?
[ ] Which device/account/service?
[ ] What exactly happens?
[ ] What should happen instead?
[ ] When did it begin?
[ ] Did it work before?
[ ] What is the scope?
[ ] What is the user impact?
[ ] What evidence exists?
[ ] Were there recent changes?
[ ] Is the issue reproducible?
[ ] What has already been tried?
[ ] What remains unknown?
[ ] Am I assuming anything without evidence?
```

---

## Next Step

Complete:

`exercises/02-request-intake-exercises.md`

before moving to:

`study-guides/03-clear-actionable-support-communication.md`
