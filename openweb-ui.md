# OpenWebUI

- OS: Debian 12 LXC
- Name: openwebui
- IP: 192.168.7.166
- Port: 8080
- URL: http://192.168.7.166:8080
- Container u/p: root / "op://Private/prox - openwebui-ct/password"
- App u/p: my email / "op://Private/prox OpenwebUI/current-password"


## Installation Options

Run this [helper script](https://community-scripts.github.io/ProxmoxVE/scripts?id=openwebui) to create a LXC and install.

Follow the prompts; enable Ollama. 

## Update Procedure

You could run the `helper script` above, I don't think that it will muck anything up. The steps below are pulled from
the steps in the script. Could be useful if you want to update either Ollama or OpenWebUI separately.

1. SSH into the container `ssh root@192.168.7.166`
1. run `apt update`
1. run `apt upgrade`
1. `cd /opt/open-webui`
1. run `git pull`
1. `cd /opt/open-webui/backend`
1. run `pip3 install -r requirements.txt -U`
1. `cd /opt/open-webui`
1. run `npm install`
1. run `npm run build`
1. restart ollama service `systemctl restart ollama`
1. check ollama service `systemctl status ollama`
1. restart openwebui service `systemctl restart open-webui`
1. check openwebui service `systemctl statu open-webui`
