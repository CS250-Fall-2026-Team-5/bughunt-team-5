Test Cases: [GP]  Team number: [5]

Test ID: 1
Written by: Grant Phillips
Title: Vote is rejected when user has 0 votes remaining
Traces to: Voting feature requirement (max votes per user)
Test type: Boundary Value / Negative
Preconditions: User is registered and logged in; voting is open; at least one costume is on the Vote page
Test data: MAX_VOTES_PER_USER = N
Steps:
1. Log in and open the Vote page
2. Click Vote on any costume N times
3. Confirm the page shows "Votes remaining: 0"
4. Click Vote once more
Expected result: Vote is blocked; message "You have used all of your votes!" appears; votes remaining stays at 0; costume vote count does not change
Actual result: Vote is accepted; costume vote count increases by 1; page shows "Votes remaining: -1"
Status: Fail
Severity: Major
V or V: Verification

Test ID: 2
Written by: Grant Phillips
Title: Vote is rejected when user is not logged in
Traces to: Voting feature requirement (only logged-in users can vote)
Test type: Negative / Authorization
Preconditions: No user is logged in (header shows "Not logged in"); voting is open; at least one costume exists
Test data: None (no session)
Steps:
1. Log out, or open the app with no active session
2. Open the Vote page
3. Click Vote on any costume
Expected result: Vote is blocked; message such as "Please log in to vote." appears; costume vote count does not change
Actual result: Vote is accepted; costume vote count increases by 1
Status: Fail
Severity: Critical
V or V: Verification