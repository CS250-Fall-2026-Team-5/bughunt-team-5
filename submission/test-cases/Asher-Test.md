Test Cases: [Asher P]
Team number: [5]

<!--
HOW TO USE THIS FILE
Copy this file. Name the copy with your first name and last initial, like  maria-g.md
Leave TEMPLATE.md untouched for your teammates.
Write at least ONE failing test case. More is better.
Copy the block between the lines for each new test case.
Test IDs: use your initials plus a number, like  MG-01, MG-02. This keeps IDs unique across your team.
See docs/TESTING_FIELD_GUIDE.md for the sample test case TC-00.
-->

---

Test ID: AP-01
Written by: Asher Plotsky
Title: Does voting close on time.
Traces to: REQ G1  REQ 13
Test type: Acceptance
Preconditions: People can not vote after 11:30 PM
Test data: Turn in vote at 11:45 PM

Steps:
Open vote
Submit vote at 11:45 PM

Expected result: Does not accept vote
Actual result: Accepts vote
Status: (Pass / Fail)
Severity: (Critical / Major / Minor, Fail only)
V or V: (Verification / Validation, Fail only)

---

Test ID: AP-02
Written by: Asher Plotsky
Title: Only owner of costume can delete
Traces to: REQ 08
Test type: Security
Preconditions: You are not owner of a costume
Test data: 

Steps:
Click delete on a costume that is not yours

Expected result: Costume not deleted
Actual result: Costume deleted
Status: Fail
Severity: Major
V or V: Verification

---

Test ID: AP-03
Written by: Asher Plotsky
Title: All categories are eligible for voting
Traces to: REQ 07
Test type: Integration
Preconditions: None
Test data: Creative costume.

Steps:
Submit a creative costume.

Expected result: Creative costume shows in vote
Actual result: Creative costume does not show up in vote
Status: Fail
Severity: Major
V or V: Verification