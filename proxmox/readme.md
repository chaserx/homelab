# Proxmox

## Installation

I ran into challenges installing Proxmox v8 directly on the [P520](../hardware/p520.md).
It would stall early on I think due to graphics driver compatibility or something like that. 

Installing Proxmos v7 and then upgrading to v8 worked just fine. 

## Nvidia Graphics Driver installation and Passthrough

### Resources

- [Setting Up a GPU-Optimized Homelab With Proxmox and Ollama](https://medium.com/@re7dworschak/setting-up-a-gpu-optimized-homelab-with-proxmox-and-ollama-1f676b609147)
- [Using an Nvidia GPU with Proxmox LXC](https://yomis.blog/nvidia-gpu-in-proxmox-lxc/)
- [Installing Nvidia Drivers on Proxmox - Gist](https://gist.github.com/Cyberes/bc33b3f4d36742ea7a036a8c7c37061e)
- [Proxmox forum on kernel pve headers](https://forum.proxmox.com/threads/upgrade-problem-to-8-2-6-8-kernel-nvidia-drivers.145749/page-2#post-664595)
- [Proxmox forum: Upgrade problem to 8.2 (6.8 kernel - nvidia drivers)](https://forum.proxmox.com/threads/upgrade-problem-to-8-2-6-8-kernel-nvidia-drivers.145749/)
- [Hardware Haven - proxmox setup walkthrough](https://www.youtube.com/watch?v=_sfddZHhOj4)
- [Debian Nvidia Graphics Drivers](https://wiki.debian.org/NvidiaGraphicsDrivers#Version_535.183.01-1)
- [Proxmox passthrough](https://sluijsjes.nl/2024/05/18/coral-and-nvidia-passthrough-for-proxmox-lxc-to-install-frigate-video-surveillance-server/)

## Docker in Proxmox

### Resources

- [Reddit thred on What's the best way to run Docker in Proxmox?](https://www.reddit.com/r/Proxmox/comments/1cluao4/whats_the_best_way_to_run_docker_in_proxmox/)
- [Portainer](https://www.portainer.io)
- [Community scripts - Docker](https://community-scripts.github.io/ProxmoxVE/scripts?id=docker-vm)
- [Reddit thread on Docker in LXC vs VM](https://www.reddit.com/r/Proxmox/comments/mmvq8h/docker_in_lxc_vs_vm/)
