# VICIDIAL INSTALLATION SCRIPTS (Default is Eastern Time Zone US)
# Centos7 and AlmaLinux Vicidial Install pre_requisites 

```

hostnamectl set-hostname xxxxxx.xxxxx.xxx
### Use YOUR SubDomain

vi /etc/hosts
##Change domain name for actual server ip (xxx.xxx.xxx.xxx   complete domain name    subdomain only)

timedatectl set-timezone America/New_York

yum check-update
yum update -y
yum -y install epel-release
yum update -y
yum install git -y
yum install -y kernel*

#Disable SELINUX
sed -i 's/SELINUX=enforcing/SELINUX=disabled/g' /etc/selinux/config    

reboot

````
  Reboot Before running this script

# Install VICIDIAL scripts

```
git clone https://github.com/carpenox/vicidial-install-scripts.git
cd vicidial-install-scripts
```

# Alma 9 Installer

```
chmod +x alma9.sh
./alma9.sh
```

# Alma 8 Add on telephony server for a cluster

```
chmod +x Vici-alma-dialer-install.sh
./Vici-alma-dialer-install.sh
```

# Execute Centos7 Vicidial Install
```
chmod +x vicidial-install-c7.sh
./vicidial-install-c7.sh
```

# Execute AlmaLinux Vicidial Install
```
chmod +x vicidial-install-almalinux.sh
./vicidial-install-almalinux.sh
```


# Install WEBRTC for VICIDIAL Now (coming soon)
# DO THIS IF YOU HAVE PUBLIC DOMAIN WITH PUBLIC IP ONLY

```
chmod +x vicidial-enable-webrtc.sh
./vicidial-enable-webrtc.sh
```
