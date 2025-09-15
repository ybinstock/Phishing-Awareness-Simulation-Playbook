# Phishing-Awareness-Simulation-Playbook


Executive Summary

Scope: Train and test all workforce members (employees, contractors with access). Simulations target only internal recipients. Integrate with your broader security awareness program.

Cadence: Quarterly company-wide simulations; monthly for higher-risk roles/teams; include new hires immediately. Increase difficulty over time.

Content: Mix of credential harvest, malicious attachment, spear-phish, and SMS/voice/QR variants; escalate realism. Pair every simulation with instant micro-training.

Report Phish: Make reporting one-click and blame-free. Route to SOC/IT Security with clear triage/escalation. Close the loop with the reporter.

Metrics: Track click-through (fail) rate, report rate, time-to-report, time-to-takedown, and repeat-offender trends. Use a dashboard and target ranges.

Standards: Aligns with NIST CSF (PR.AT, DE.AE, RS.CO) and ISO 27002 (5.10, 5.30).

0) Quick Start

Publish this playbook and announce the program.

Enable a one-click Report Phishing button (Outlook/GWS) and create a security mailbox (e.g., phish@acme.example).

Run a baseline easy simulation + instant micro-training.

Launch a short phishing module for all staff; enroll new hires automatically.

Set a quarterly all-hands cadence + monthly targeted drills.

Stand up a metrics dashboard (see §5). Iterate each quarter.

1) Scope Definition

In-scope:

Employees, contractors, interns, and vendors with corporate email or SSO access.

Corporate mail domains only; exclude external customers/partners from simulation sends.

Out-of-scope:

Personal mailboxes; external mailing lists; public/contact-us inboxes (unless explicitly approved).

Integration with Awareness Training

Deliver a short phishing module during onboarding; refresh annually.

Pair every simulation with on-click micro-training (“teachable moment” landing pages).

Use simulation results to trigger targeted refreshers and coaching.

Objectives (set per campaign)

Reduce click rate; increase report rate; shorten time-to-report.

Stress-test response workflows (triage, takedown).

Exercise high-risk roles (Finance, HR, EA/Leadership, IT/Admins).

Governance & Approvals

Obtain CISO/IT lead + Legal approval for scope/timing.

Notify Helpdesk/Mail admins before each campaign.

Document all campaigns (who/when/templates/metrics).

2) Cadences

Company-wide:

Quarterly simulation (4×/year), difficulty increases each quarter.

Avoid predictable days/times; vary lure types.

High-risk roles/teams (Finance, HR, EA, IT):

Monthly targeted drills (e.g., invoice fraud, W-2 requests, password reset spoofs).

Include occasional cross-channel variants (SMS/voice/QR).

New Hires / Role Changes:

Enroll within 2 weeks of start or role elevation; run a simple simulation plus onboarding module.

Adaptive Tuning:

Frequent clickers: add micro-coaching and lighter-weight remediation simulations.

High performers: advance to harder templates (closer to real threats).

Watch fatigue signals; prioritize quality over quantity.

Difficulty Progression (year 1 example):

Q1: Obvious generic lures (spelling mistakes, weird senders).

Q2: Brand-impersonation and tool notices (SharePoint, DocuSign).

Q3: Role-targeted spear-phish (CFO/AP wire, HR résumé).

Q4: Advanced multi-step (QR code, callback/vishing, MFA fatigue).

3) Content Map (with Examples)
A) Generic (broad, low sophistication)

Credential Harvest — “Password Expiry”

Attachment — “Unpaid Invoice”

Account Notice — “Mailbox Quota”

B) Targeted (role-specific, internal context)

BEC — “CFO Wire Transfer (Urgent/Confidential)”

HR — “Candidate Résumé”

Internal Tools — “Ticket Closed / File Share”

C) Advanced (modern tradecraft)

MFA Fatigue / Approval Bombing

Quishing — “Scan QR to View Secure Doc”

Callback/Vishing — “Auto-Renewal $399 — Call to Cancel”

D) SMS (“Smishing”) & Chat (optional add-ons)

SMS — “Payroll Portal Lock”

Chat — “IT Security” in Teams/Slack”

4) “Report Phish” Flow

User Experience

One-click Report Phishing button in Outlook/Gmail.

Confirmation: “Thanks—Security is investigating.”

Blame-free culture.

Back-End Routing

Forward to security mailbox/analysis.

Auto-create ticket.

Triage (simulation vs. benign vs. malicious).

Contain/remove if malicious.

Reset creds/check devices if clicked.

Close loop with reporter.

Escalation & SLAs

Triage start: within 15 min.

Containment: within 60 min.

Simulation debrief: same day.

5) Metrics & Dashboard
Metric	Definition	Target
CTR	% who clicked	<5–10% routine
Report Rate	% reported	>CTR; 20–30%+
Report:Click Ratio	Reports ÷ Clicks	>1.0
Time-to-Report	Delivery → first report	≤60 min
Time-to-Takedown	First report → containment	≤60 min
Repeat Clickers	Users with ≥2 fails	Declining
Training Completion	% training done	≥95%
6) Awareness vs. Simulation

Awareness

Short modules, tip sheets, manager talking points.

Promote Report button.

Positive recognition.

Simulation

Vary lures and difficulty.

Teachable landing pages.

No shaming; targeted remediation.

Feed results into IR.

7) Templates & Snippets (Fictional)

Campaign Announcement

Next week Acme will run a phishing drill. Please use Report Phishing. No blame.

Report Acknowledgement

Thanks for reporting. Our security team is investigating.

Real Threat Advisory

We are seeing payroll-themed phish. Do not click. Report immediately.

Teachable Landing Page

This was a simulation. Red flags: mismatched domain, urgent tone.

8) Roles & RACI
Activity	Employee	Manager	Helpdesk	SOC/IR	Mail Admin	Legal/Comms
Recognize & Report	R	A	C	C	C	I
Triage & Classify	I	I	C	R/A	C	I
Contain & Takedown	I	I	C	R	A	I
User Notification	I	I	C	R	I	A
Training Content	R	A	I	C	I	C
Program Governance	I	I	I	R	C	C
9) Standards Alignment

NIST CSF: PR.AT, DE.AE, RS.CO

ISO 27002: 5.10 (Awareness), 5.30 (ICT Continuity)

10) Roadmap (First 2 Quarters)

Month 1: Enable Report button, baseline test, module.

Month 2: Targeted Finance/HR drill, dashboard v1.

Month 3: Company-wide moderate test.

Month 4: Add SMS/QR awareness tip, pilot QR drill.

Month 5: Finance/AP BEC drill.

Month 6: Company-wide spear-phish drill, publish Q2 metrics.

11) Appendix — Risk Register Seeds

PH-01: Low Report Rate Region A → re-promote button.

PH-02: High CTR AP Team → refresher training.

PH-03: Slow Takedown → automate mailbox purge.

PH-04: Repeat Clickers → 1:1 micro-coaching.
