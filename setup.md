
# Lab Setup and Verification

## Environment
- Host OS: Linux
- Container runtime: Docker
- Target: OWASP Juice Shop
- Container: `juice-shop-lab`
- Network: `ethical-lab`

## Setup
The Juice Shop application runs inside a Docker container connected to an internal Docker bridge network. The intended host access is through `127.0.0.1:3000`.

## Verification Commands
```bash
sudo docker ps
sudo docker network inspect ethical-lab
sudo docker inspect juice-shop-lab
sudo docker port juice-shop-lab
curl -I --max-time 5 http://127.0.0.1:3000
```

## Evidence
- `evidence/lab-running.png`: application screenshot.
- `evidence/network-isolation.png`: Docker network configuration screenshot.

## Verification Status
The internal network is configured with Docker's `Internal` setting enabled. The localhost port access must also be tested successfully before marking the website access and complete isolation as verified.

## Cleanup
Stop the application when finished:
```bash
sudo docker stop juice-shop-lab
```
