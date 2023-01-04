
We create a .repo file within /etc/yum.repos.d using a text editor. In this example, we will create the repository file for MySQL 5.7

Step1 :
cd /etc/yum.repos.d/

Step2:
vim mysql57-community.repo
[mysql57-community]
name=MySQL 5.7 Community Server
baseurl=http://repo.mysql.com/yum/mysql-5.7-community/el/7/$basearch/
enabled=1
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql

Step3:
yum-config-manager mysql57-community [ Validate the yum repository ] 

Step4:
yum install mysql
