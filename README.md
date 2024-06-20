# Cortex-XDR-Agent
### Install the Cortex XDR agent for Rocky Linux.
- **tar xf SPX_Linux_sh.tar.gz**
- **vi cortex.conf**
- copy **--proxy-list="vnsgnsxdr1:8888,vnsgnsxdr2:8888"**
- **sudo mkdir -p /etc/panw**
- **sudo cp cortex.conf /etc/panw/**
- **sudo yum -y install selinux-policy-devel**
- **chmod +x cortex-8.2.0.118335.sh**
- **./cortex-8.2.0.118335.sh**
- **/opt/traps/bin/cytool runtime stop all**
- **/opt/traps/bin/cytool runtime start all**



