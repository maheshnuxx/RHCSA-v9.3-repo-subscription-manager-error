# RHCSA-v9.3-repo-subscription-manager-error
in RHCSA v9.3 this repository is not registered in subscription-manager problem solve in this 

i complete my RHCSA (Redhat certified system administrator) in 14 may 2026 but this is my 2nd attempt , in my first attemp i have error in RHCSA exam 2nd task repository thats why my other task like Container , Autofs , and other task that they need to download and configure not completed <br>
 # This repository is not registerd in Subscription-manager -----{error}

and in my second aatemp i solve them its very easy <br>
let's start
# commands

#yum repolist all <br>
this repository is not registered in subscription-manager -------{this error comes then next step}

#yum clean all <br>
#vim /etc/yum/pluginconf.d/subscription-manager.conf <br>

{then we find enabled=1  change this 1 into 0 } <br>
before -- enabled=1 <br>
after -- enabled=0 <br>
{off the subscriptiom-manager} <br>

esc + :wq <br>


#yum clean all <br>
#yum repolist all <br>
#vim /etc/yum.repos.d/exam.repo <br>

[BaseOS] <br>
name=BaseOS <br>
baseurl=server1.net17.example.com/BaseOS <br>
gpgcheck=0 <br>
enabled=1 <br>

[AppStream] <br>
name=AppStream <br>
baseurl=server1.net17.example.com/AppStream <br>
gpgcheck=0 <br>
enabled=1 <br>

esc + :wq <br>

#yum repolist all <br>
#yum install tree -y <br>

Its is full solution of RHCSA v9.3 repository task , all the best for exam 
