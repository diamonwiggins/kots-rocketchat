# RocketChat KOTS Appliance
This repository houses all the config needed to deploy a RocketChat KOTS appliance

Once the KOTS appliance has been successfully deployed, the app will be available via https over the standard port.(eg. https://your-dns.example.com)

## Preflight Checks
Checks that must pass before the KOTS appliance can come online
- K8s cluster version must be higher than `1.15.0`
- 1 CPU core required. 2 CPU cores recommended
- 1GB of RAM required. 2GB of RAM recommended
- 20GB of disk capacity for the root partition required. 40GB recommended

## Config Options
- RocketChat DNS Hostname
- Mongo Root Password
- Mongo RocketChat Password
- Mongo Volume Size

## Support Bundle
- Retrive cluster info and resources
- Retrieve RocketChat API health status
- Retrive MongoDB version
- Ping Google DNS address
- Ping Google IP Address

## Helm
RocketChat Helm chart forked to use Contour's HTTPProxy object as opposed to traditional Ingress
