# Installing-and-configuring-Jenkins

Step to setup Jenkins in a Linux environment-

*As Root*
```

1. Update package list, install Java runtime environment and verify the install.
$ apt update 
$ apt install openjdk-8-jdk 
$ java -version 

2. Install Jenkins.
$ wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add - 
$ sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
$ sudo apt install jenkins 
$ sudo service jenkins status 

3. Start Jenkins.
$ sudo /etc/init.d/jenkins start 

4. Open localhost:8081 in browser.

5. Copy paste the admin password
$ cat jenkins/secrets/initialAdminPassword

6. Select suggested plugins after entering password. You can create the admin user id, password and start using Jenkins!

```
*As Root*
