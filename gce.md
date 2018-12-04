CentOS Linux release 7.5.1804 (Core) 

yum install epel-release -y
yum install gcc gettext autoconf libtool automake make pcre-devel asciidoc xmlto c-ares-devel libev-devel libsodium-devel mbedtls-devel -y
systemctl stop firewalld.service
systemctl disable firewalld.service
yum install wget
rpm -ivh https://buildlogs.centos.org/c7.1511.00/kernel/20151119220809/3.10.0-327.el7.x86_64/kernel-3.10.0-327.el7.x86_64.rpm --force
awk -F\' '$1=="menuentry " {print $2}' /etc/grub2.cfg 
grub2-set-default 0
shutdown -r now
wget -N --no-check-certificate https://softs.fun/Bash/ssrmu.sh &&chmod +x ssrmu.sh &&bash ssrmu.sh
./ssrmu.sh 


 I  P       : 35.229.188.151
 端口       : 9327
 密码       : Elabxha123
 加密       : salsa20
 协议       : origin
 混淆       : plain
