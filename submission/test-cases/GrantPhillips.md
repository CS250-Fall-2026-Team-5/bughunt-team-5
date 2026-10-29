Test Cases: [GP]
Team number: [5]

Test ID: 1
Written by: Grat Phillips
Title: User can vote when 0 votes remain
Traces to: Voting feature requirement
Test type: Boundary Value / Negative
Preconditions: User can vote with 0 votes left
Test data: 0 votes left but when user votes there is -1 votes left

Steps:

Expected result: Vote is blocked; user sees a message like "No votes remaining" and vote count stays at 0
Actual result: Vote is accepted; user's vote count becomes -1
Status: Fail
Severity: Major
V or V: Validation


Test ID: 2
Written by: Grat Phillips
Title: User can vote when not signed in
Traces to: Voting feature requirement
Test type: Boundary Value / Negative
Preconditions: User can vote without being logged in
Test data: Account voting yet they are not even signed in

Steps:

Expected result: Vote is blocked; user sees a message like "Cant vote your not logged in".
Actual result: Vote is accepted
Status: Fail
Severity: Major
V or V: Validation
