Test Plan for End-to-End Testing
Scope
This test plan covers the functional, security, and performance testing for the xaltsocnportal.web.app CRUD blockchain application. It focuses on user actions such as Sign Up, Sign In, Request Submission, and Sign Out.

Types of Tests & Purpose
Type of Test	                                                             Description
Functional Testing	                Verifies that all features (Sign Up, Sign In, Submit Requests)
Boundary Testing	                  Ensure input fields handle edge cases for data types
Negative Testing	                  Confirm system handles invalid data gracefully without crashes.
UI/UX Testing	                      Assess user experience and UI components for usability.
Integration Testing	                Interactions between components such as wallet addition & blockchain onboarding requests.
Performance Testing	                Assess system speed and stability under different user loads.
Security Testing	                  Evaluate application against common vulnerabilities like XSS, CSRF, and data leaks.


Test Cases for Success and Failure Scenarios

Sign Up Tests

•	Success Scenario
o	Valid email and password format
o	Password meets complexity requirements
o	Account creation is successful with confirmation message

•	Failure Scenarios

o	Invalid email format
o	Password too short or lacks complexity
o	Email already registered
o	Blank email or password

Sign In Tests

•	Success Scenario

o	Correct credentials log the user into the system

•	Failure Scenarios
o	Incorrect password
o	Unregistered email
o	Blank email or password

Onboard Node Request Tests

•	Success Scenario

o	Valid Node ID (NodeID-1) and IP address (192.168.1.1)
o	Multiple nodes added successfully
o	Valid wallet addresses and permissions

•	Failure Scenarios

o	Invalid Node ID or public IP address
o	Duplicate Node IDs
o	Wallet address format validation errors (0x prefix missing)
o	Submitting an empty list of nodes or wallets

New Private Blockchain Request Tests

•	Success Scenario

o	Network name and wallet are valid
o	Nodes added successfully
o	Submission succeeds

•	Failure Scenarios
o	Invalid network name format
o	Wallet address validation errors
o	Submission without any nodes

Sign Out Tests
•	Success Scenario

o	User is logged out and redirected to the login screen
•	Failure Scenario

o	Attempting to access private routes after logging out
