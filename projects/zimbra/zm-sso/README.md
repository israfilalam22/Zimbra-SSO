Zimbra Single Sign On (Zm SSO)
=========================================
Zm SSO is the Zimbra Collaboration Open Source Edition extension for single sign-on authentication to the Zimbra Web Client.  
Copyright (C) 2020-present iWay Vietnam and/or its affiliates. All rights reserved.

* Using framework: [pac4j](https://www.pac4j.org) is an easy and powerful security engine for Java to authenticate users,
  get their profiles and manage authorizations in order to secure web applications and web services.
* Supported authentication mechanisms: [SAML](http://www.pac4j.org/docs/clients/saml.html) -
  [CAS](http://www.pac4j.org/docs/clients/cas.html) -
  [OpenID Connect](http://www.pac4j.org/docs/clients/openid-connect.html)

## Building Java extension
### Requirement
* JDK 11 or newer.
* Apache Maven 3.5 or newer for Maven build.

### Setting up your build system
* On Fedora or CentOS 8.x or Red Hat EL 7.x
```shell
dnf -y install java-11-openjdk java-11-openjdk-devel maven ant git make rpmdevtools rpm-build
```
* On CentOS 7.x or Red Hat EL 7.x
```shell
yum -y install java-11-openjdk java-11-openjdk-devel maven ant git make rpmdevtools rpm-build
```
* On Debian or Ubuntu
```shell
apt install -y openjdk-11-jdk maven ant git make
```


### Clone code from git repository
```shell
mkdir -p ~/projects/zimbra
cd ~/projects/zimbra
git clone https://github.com/iwayvietnam/zm-sso.git
```

### Build jar file by using Maven
```shell
cd ~/projects/zimbra/zm-sso
mvn clean package
```
The output should be like this:
```
--- maven-jar-plugin:3.0.2:jar (default-jar) @ zm-hab ---
Building jar: ~/projects/zimbra/zm-sso/target/zm-sso-1.0.0-1.jar
```
