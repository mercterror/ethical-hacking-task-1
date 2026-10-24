# Legal Scope and Isolated Lab

**Track:** Ethical Hacking  
**Level:** Beginner  
**Target:** OWASP Juice Shop

## Project Overview
This project establishes a local practice environment for learning ethical hacking and web application security.

## Topology
Linux Host → Docker Runtime → Internal Docker Network (`ethical-lab`) → OWASP Juice Shop

The application is published on the host's loopback interface. The actual network configuration must be verified before claiming that the lab is isolated.

## Scope
Only the locally controlled Juice Shop instance is authorized for testing.

## Safety
Unauthorized systems, public networks, destructive testing, and denial-of-service activities are excluded.

## Evidence
The `evidence/` folder contains screenshots of the local application and network verification.

## Completion
The lab is considered complete after setup, isolation verification, documentation, and evidence capture.
