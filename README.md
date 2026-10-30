cd ~/ethical-hacking-task-1

cat > README.md <<'EOF'
# Ethical Hacking Task 1 – Legal Scope and Isolated Lab

## Overview
An isolated ethical hacking environment using Docker and OWASP Juice Shop for authorized security testing.

## Lab Details
- OS: Linux
- Container: juice-shop-lab
- Application: OWASP Juice Shop
- Docker Network: ethical-lab
- Network Type: Internal
- Target: http://127.0.0.1:3000

## Network Topology
Linux Host → Docker Runtime → Internal Docker Network → OWASP Juice Shop

## Scope
Testing is restricted to the locally hosted Juice Shop application.

## Rules of Engagement
See [RULES_OF_ENGAGEMENT.md](RULES_OF_ENGAGEMENT.md).

## Evidence
- evidence/lab-running.png
- evidence/network-isolation.png

## Cleanup
Stop the container:

```bash
sudo docker stop juice-shop-lab