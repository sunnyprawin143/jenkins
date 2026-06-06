<img width="1287" height="507" alt="image" src="https://github.com/user-attachments/assets/fb716608-c0aa-41e7-b820-a2b60fb08df1" />install java lastest version
**yum install java-21-amazon-corretto -y**
java --version  to check java installed
go to **jenkins.io** and click on **download** option available on top right
under LTS we have below options available:
Docker
Kubernetes
Ubuntu/Debian
**Red Hat Enterprise Linux and derivatives**
Fedora
Windows
openSUSE
**among these select red hat linux since i opt amazon linux os while creating instance creation**

afrer selecting red hat we see below steps in that page:
step1: download jenkins repo

sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/rpm-stable/jenkins.repo

step2: download jenkins
yum install jenkins -y

after successful installation we can see the _**jenkins key generated
**_

step3: start jenkins
systemctl start jenkins

step4:
copy the public key of instance and browse along with port number 8080

example: 13.235.81.245:8080
it will give the unlock jenkins page and specify the password saved path 
cat that path and get the password to log in

/var/lib/jenkins/secrets/initialAdminPassword
example:0477d288f21848a8b5842a769f5a106d

after login click on suggested install
then it will all required packages



