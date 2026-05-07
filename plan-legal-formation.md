# Plan — P1: Legal & Business Formation

**Level:** 5 — Plan
**Parent Project:** P1 — `projects.md`
**Parent Goal:** Studio Goal — `project_aurora.md`
**Built:** 2026-05-03
**Status:** Active

---

## Milestones

### M1 — Missouri LLC Registered
*State: Articles of Organization filed and stamped copy received from Missouri SOS. Studio name confirmed available.*

**Dependencies:** None — no external conditions required to begin.

### M2 — Federal Identity Established
*State: EIN obtained from IRS. CP 575 confirmation notice downloaded and saved.*

**Dependencies:** M1 complete. IRS requires confirmed state formation before EIN application. (Exception: see Decision Rules — EIN prep can begin in parallel if M1 submission is delayed.)

### M3 — Legal & Financial Foundation Complete
*State: Operating Agreement executed and signed. Business bank account open at FCCU or equivalent. BOI filing exempt — FinCEN rule change (2026) removes requirement for U.S. domestic entities.*

**Dependencies:** M2 complete. Bank account requires EIN.

### M4 — Distribution Accounts Configured
*State: Steam developer account active — NDA and Distribution Agreement signed, $100 app fee paid, tax interview complete, bank account linked. itch.io developer account created. Epic Games Store account created (if applicable).*

**Dependencies:** M3 complete. Steam tax interview and payout setup require EIN and business bank account.

---

## Sequencing

```
M1 → M2 → M3 → M4
```

All milestones are strictly sequential. No milestone generates tasks until the preceding milestone is closed. Exception noted in Decision Rules below.

---

## Dependencies

| Dependency                                                 | Type      | Required By             | Status                          |
| ---------------------------------------------------------- | --------- | ----------------------- | ------------------------------- |
| Studio name available in Missouri Business Entity Database | Internal  | M1                      | ✓ Confirmed                     |
| Missouri SOS online account                                | Internal  | M1                      | ✓ Created                       |
| IRS EIN online application window (Mon–Fri, 7am–10pm ET)   | External  | M2                      | Scheduling constraint only      |
| Stamped Articles of Organization                           | M1 output | M2, M3                  | ✓ Received and saved 2026-05-04 |
| EIN / CP 575                                               | M2 output | M3, M4                  | ✓ Obtained and saved 2026-05-04 |
| Operating Agreement (executed)                             | M3 output | Bank account            | ✓ Executed and saved 2026-05-05 |
| Business bank account                                      | M3 output | M4 Steam/Epic tax setup | ✓ Open 2026-05-05               |

---

## Decision Rules

- **Name conflict at M1:** Have 2 backup studio names ready before opening the SOS portal. Do not proceed to Articles of Organization without a confirmed available name.

- **M1 SOS processing delay (>2 weeks from submission):** Begin IRS EIN prep in parallel — the IRS application does not require the stamped copy in hand, only that formation has been submitted. Tag EIN tasks with `dependency: awaiting_M1_confirmation` and complete the application up to (but not including) submission until M1 formally closes.

- **FCCU unavailable for M3 bank account:** Do not block M3 completion on a single institution. Any business-capable bank or credit union accepting Missouri LLC documentation is an acceptable fallback. Log the substitution in the Review Notes on `projects.md`.

- **Budget constraint at M4 Steam fee ($100):** If the $100 app fee is not available at M4 time, minimum viable M4 completion is: itch.io developer account created (free) + Steamworks account created (free, separate from the paid App submission). Steam distribution is unlocked later as a follow-on task. Do not block M4 closure on the Steam fee.

- **M4 Epic Games Store:** Optional at this stage. Include only if setup can be completed without extending M4 timeline. If it creates friction, archive to backlog and tag for P2 or pre-launch checklist.

---

## Plan Execution Log

*Updated when milestones close or decision rules are triggered.*

| Date       | Milestone | Event                                       |
| ---------- | --------- | ------------------------------------------- |
| 2026-05-03 | —         | Plan built. M1 tasks generated in tasks.md. |
| 2026-05-04 | M1        | Closed. All 7 tasks completed. Stamped Articles of Organization received. M2 tasks generated in tasks.md. |
| 2026-05-04 | M2        | Closed. All 5 tasks completed. EIN obtained and confirmation saved. M3 tasks generated in tasks.md. |
| 2026-05-05 | M3        | Closed. Operating Agreement executed, business bank account open. BOI tasks voided — FinCEN rule change exempts U.S. domestic entities from beneficial ownership reporting. M4 tasks generated in tasks.md. |
| 2026-05-05 | M4        | Closed. Steamworks account active, Distribution Agreement signed, $100 fee paid, tax interview complete, bank linked. itch.io and Epic Games Store accounts created. P1 fully closed. P2 and P3 activated in projects.md. |
