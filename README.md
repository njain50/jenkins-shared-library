# jenkins-shared-library
sample jenkins shared library to automate jobs in pipeline

(1) install jenkins on windows ==>

(a) download msi from here: https://www.jenkins.io/download/thank-you-downloading-windows-installer-stable/
(b) login with admin and password here: file:///C:/WINDOWS/system32/config/systemprofile/AppData/Local/Jenkins.jenkins/secrets/initialAdminPassword
(c) Install suggested plugins
(d) set credentials: admin/admin
(e) jenkins URL: http://localhost:8080/

(2) Configure Azure VM as slave

(a) login to VM as root
(b) mkdir -p /cs/devtooling/jenkins/ws
(c) sudo useradd -d /var/lib/jenkins jenkins , passwd jenkins 
(c) if swap if zero, can refer here https://ghanshammahajan.com/how-to-add-a-swap-space-in-linux-azure-virtual-machines/
(d) Manage Jenkins ==> Manage Node ==> New Node ==> azurevm
(e) install following packages on ubuntu azure vm: sudo apt-get install openjdk-8-jre
(f) Refer here https://yallalabs.com/devops/how-to-add-linux-slave-node-agent-node-jenkins/ for final configuration. 

(3) 
 


