Test Cases: [GP]  Team number: [5]

Test ID: 1
Written by: Grant Phillips
Title: Can't vote with 0 votes left
Traces to: Voting requirement
Test type: Boundary Value / Negative
Preconditions: User is logged in
Test data: User has 0 votes left
Steps:
1. Log in and go to the Vote page
2. Use all your votes
3. Click Vote one more time
Expected result: Vote is blocked and a "no votes left" message shows
Actual result: Vote goes through and votes left shows -1
Status: Fail
Severity: Major
V or V: Verification

Test ID: 2
Written by: Grant Phillips
Title: Can't vote without logging in
Traces to: Voting requirement
Test type: Negative
Preconditions: User is not logged in
Test data: None
Steps:
1. Make sure you are logged out
2. Go to the Vote page
3. Click Vote on any costume
Expected result: Vote is blocked and a "please log in" message shows
Actual result: Vote goes through
Status: Fail
Severity: Major
V or V: Verification