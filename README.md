# TESTS

Once you provision vagrant servers
1- install python3 on jump server and install --> yum install libselinux-python3-2.5-15.el7.x86_64 -y
2- create key pair and add it to its own authorized_keys on jumpserver
3- create this key pair also as root and add it to all other servers  /root/.ssh/authorized_keys 
4- install the collections below on jumpserver to be able to run the yml 
    ansible-galaxy collection install community.general
    ansible-galaxy collection install ansible.posix 
5- /etc/selinux/config change selinux config to permisive


