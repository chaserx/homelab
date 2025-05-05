# Tailscale 

## Installation options

### Community Helper Script

Installed by this [helper script](https://community-scripts.github.io/ProxmoxVE/scripts?id=add-tailscale-lxc)

After the script finishes run `tailscale up`.

### Official Installation Documentation

https://tailscale.com/kb/1031/install-linux

## Current configuration

- Debian 12 LXC
- Name: tailscale-ct
- IP: `192.168.7.191`
- u/p: root / "op://Private/proxmox tailscale-ct/password"
- Options: Disable Key Expiry; advertises subnets; offers exit node

## Update Procedure

- run `apt update`
- run `apt upgrade`
- reboot lxc
- run `tailscale up` or `tailscale up --accept-routes --advertise-exit-node`

## Resources

- [YouTube: Tailscale inside LXC](https://youtu.be/QJzjJozAYJo?si=8oGuDrllNVLyhAoh)
- [HOW TO ACCESS MULTIPLE LXC CONTAINERS THROUGH A SINGLE TAILSCALE CONNECTION](https://diegocarrasco.com/access-multiple-lxc-containers-single-tailscale/)
