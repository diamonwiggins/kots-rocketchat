# RocketChat KOTS Appliance
This repository houses all the config needed to deploy a RocketChat KOTS appliance

## Installation Steps

1. Downlaod and run the cluster installation script
```bash
curl -sSL https://k8s.kurl.sh/rocketchat | sudo bash
```
2. Follow the instructions provided at the completion of the installation script
3. Wait for the app to start successfully, and then navigate to the DNS Hostname you provide on the Config page via the browser.
```bash
https://your-dns.example.com
```

## Preflight Checks
Checks that must pass before the KOTS appliance can come online
- K8s cluster version must be higher than `1.15.0`
- 1 CPU core required. 2 CPU cores recommended
- 1GB of RAM required. 2GB of RAM recommended
- 20GB of disk capacity for the root partition required. 40GB recommended

## Config Options
- RocketChat DNS Hostname
- MongoDB Root Password
- MongoDB RocketChat Password
- MongoDB Volume Size

## Support Bundle
- Retrieve cluster info and resources
- Retrieve RocketChat API health status
- Retrieve MongoDB version
- Ping Google DNS address
- Ping Google IP Address

## Helm
RocketChat Helm chart forked to use Contour's HTTPProxy object as opposed to traditional Ingress
