# Cortex-XDR-Agent
### Install the Cortex XDR agent software.
You can install the Cortex XDR agent on the endpoint manually using the shell installer or using the Linux package manager for .rpm and .deb installers.
Unpack the installation archive by running.

- **tar xf filename.tar.gz**

Copy the configuration file into /etc/panw directory.

- **sudo mkdir -p /etc/panw**

- **sudo cp cortex.conf /etc/panw/**

### INSTALL COMMAND

#### 1. RHEL, CentOS, or Oracle   
- **yum install ./filename.rpm or rpm -i ./filename.rpm**

#### 2. Ubuntu or Debian
- **apt-get install ./filename.deb or dpkg -i ./filename.deb**

#### 3. SUSE
- **zypper install ./filename.rpm or rpm -i ./filename.rpm**

### Verify the agent was installed on the endpoint.

Enter the following command on the endpoint:

- **dpkg -l | grep cortex-agent or rpm -qa | grep cortex-agent**

## To deploy the shell installer:

- Enable execution of the script using the chmod +x filename command.

- Run the install script as root or with root permissions.

### For example on CentOS 7:  

**chmod +x cortex-7.7.0.59559.sh**  
**./cortex-7.7.0.59559.sh**
## NOTE: 
### If you are using rpm, deb or sh installers, you must also add these parameters to the /etc/panw/cortex.conf file prior to installation.

Make sure to remove the first couple of leading double dashes. For example, instead of :-- --proxy-list ”<proxyserver>:<port>”, add this: --proxy-list="10.196.21.223:808"
