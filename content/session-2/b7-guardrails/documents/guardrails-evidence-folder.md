# Guardrails Evidence Folder: ClaimAssist v3

**Fictional - for training only. Vendor and documents are made up.**

**Vendor:** Nimbus AI Solutions Ltd
**Attached to:** the guardrails section of the ClaimAssist v3 proposal
**Today's date for this exercise:** 25 November 2026

The vendor was asked to back each statement with evidence. This is what it sent.

---

## For G1: Access controls

**Settings screenshot, October 2026.** Taken from the vendor's support console for a company test account.

- Permission mode: "Team level".
- Description under the setting: "Users can see all claims opened by their team."

No test report was attached.

---

## For G2: Input filters

**Filter rule list (one page, undated).**

- The filter blocks documents that contain the exact phrases "ignore previous instructions" and "disregard the above".
- No other rules are listed.

No test results were attached.

---

## For G3: Data-loss prevention

**Rule list (one page, March 2026).** Blocks card numbers and bank account numbers.

**Test summary (March 2026).** 20 test messages written by the vendor.

| Message type | Number | Blocked |
| --- | --- | --- |
| Contains a card number | 6 | 6 |
| Contains health details | 8 | 0 |
| Clean message | 6 | 0 |

**Dashboard note (screenshot, October 2026).** "Messages blocked in the last 90 days: 0."

---

## For G4: Output filters

**Test report (2025, vendor-run).** Tested the output filter on 300 general messages for abusive or harmful language. Result: 99% handled correctly.

No test covered wrong cover statements, invented promises or letters with the wrong amount.

---

## For G5: Human approval

**Settings screenshot, October 2026.**

- Setting: "Require approval before sending letters". Default: off.
- Other actions listed: "Update claim status" and "Change payment details". Approval setting for these: "Not available".

No review statistics were attached.

---

## For G6: Monitoring and audit trail

**Sample log entry.** Fields: time, user, question, answer. Not recorded: the model version, the sources used, the hidden instructions in force.

**Retention.** Action records are kept for 7 days in the claims system.

**Dashboard screenshot, February 2026.** Counts of messages per day. No alert rules are shown.

---

## For G7: Escalation

**Incident procedure (one page).** Says incidents are "escalated to the right team". No names, roles or response times are given.

**Stop switch.** "Available through vendor support. Response within one business day."
