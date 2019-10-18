# jenkins

## Requirements
* java

## Install java

```bash
  $ yum install java-1.8.0-openjdk
```
- add the JAVA_HOME variable into the .bash_profile and change the path to include also JAVA_HOME variable.
```bash
  JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.222.b10-1.el7_7.x86_64
  PATH=$PATH:$JAVA_HOME:$HOME/.local/bin:$HOME/bin
```
## Install Jenkins on a CentOS/7 

```bash
  $ wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
  $ rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
  $ yum install -y jenkins
  $ systemctl enable jenkins
  $ systemctl start jenkins
```

