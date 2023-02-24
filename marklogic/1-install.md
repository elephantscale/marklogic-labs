# Marklogic 11 install (Amazon Linux 2)

In this lab we will practice the installation of Marklogic.


### STEP 1: Login to the lab machine

Each student is provided their individual server and credentials

(Instructor: use our ubuntu AMI, t2.large or t2.xlarge instances and Elasticsearch security group)

### STEP 2: Install marklogic

* Download .rpm jar from the below link, and sign up for free downloads:
https://developer.marklogic.com/products/marklogic-server/11.0

* Open Termial in lab machine
* cd to location where MarkLogic-11.0.0-rhel.x86_64.rpm is downloaded
    - cd Downloads/
* change user to root with cmd:
    - sudo su
* Check the status of the Universe distribution component:
    - sudo add-apt-repository universe
* Update repositories with:
    - sudo apt-get update
* The following command installs the Alien conversion tool:
    - sudo apt-get install alien
* 



```bash
wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -
```

* You may need to install the apt-transport-https package on Debian before proceeding: (I did it)

```shell
sudo apt-get install apt-transport-https
```

* Save the repository definition to /etc/apt/sources.list.d/elastic-8.x.list:

```shell
echo "deb https://artifacts.elastic.co/packages/8.x/apt stable main" | sudo tee -a /etc/apt/sources.list.d/elastic-8.x.list
```

* Run sudo apt-get update and the repository is ready for use. You can install it with:

```shell
sudo apt-get update && sudo apt-get install logstash
```

* Verify that it is installed: proceed to your [first pipeline](2-first-pipeline.md).

