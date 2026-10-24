# Rules of Engagement — Ethical Hacking Task 1

## Objective
Create a controlled lab for learning web application security without testing unauthorized systems.

## Authorized Target
- Application: OWASP Juice Shop
- URL: http://127.0.0.1:3000
- Environment: Local Docker container
- Network: Internal Docker network named ethical-lab

## Allowed Activities
- Manual website inspection
- HTTP request and response analysis
- Non-destructive input validation tests
- Authentication and security configuration checks
- Recording findings and remediation suggestions

## Exclusions
- Public websites and IP addresses
- Other people's devices and networks
- Production systems
- Any target without explicit authorization
- Denial-of-service and destructive testing
- Collection or publication of real sensitive data

## Stop Conditions
Stop immediately if traffic reaches an unauthorized target, the target identity is uncertain, sensitive information is discovered, or the host or application becomes unstable.

## Evidence Handling
Store screenshots and notes that demonstrate the lab setup. Remove credentials, tokens, and personal information before publishing evidence.

## Cleanup
Stop the container after testing. Remove the container and network when they are no longer needed.

## Authorization
Permission is limited to this locally controlled practice environment. No permission is granted to test other systems.

## Verification Status
Mark the lab operational only after verifying the actual network configuration and saving evidence.
