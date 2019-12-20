# Devops/SRE interview preparation questions
This repo is agregated guide for preparation to Devops/SRE engineer interview 

## Linux 

<details>
<summary>What is Linux Standart Base?</summary><br><b>
Explanation: https://en.wikipedia.org/wiki/Linux_Standard_Base
</b></details>

<details>
<summary>Popular Linux Distributions</summary><br><b>
The most popular linux distrs:
  
  * Ubuntu  
  * Centos  
  * Fedora  
  * Debian  
  * OpenSuse  
  * ArchLinux  
  * Slackware  
  
Comparison: https://www.howtogeek.com/191207/10-of-the-most-popular-linux-distributions-compared/
  
</b></details>

<details>
<summary>Linux boot process: from power up to login promt</summary><br><b>
Explanation: 
  
  * BIOS
  * MBR
  * GRUB
  * Kernel
  * Init
  * Runlevel
  
  https://www.thegeekstuff.com/2011/02/linux-boot-process/
</b></details>

<details>
<summary>What is inode?</summary><br><b>
Explanation: https://linoxide.com/linux-command/linux-inode/
</b></details>

<details>
<summary>Memory types in Linux</summary><br><b>
  
Explanation: https://linux-audit.com/understanding-memory-information-on-linux-systems/
</b></details>

<details>
<summary>What is sticky bit?</summary><br><b>
Explanation:
  
  * https://en.wikipedia.org/wiki/Sticky_bit
  * https://www.geeksforgeeks.org/setuid-setgid-and-sticky-bits-in-linux-file-permissions/
</b></details>

<details>
<summary>What is Virtual memory?</summary><br><b>
Explanation: 
  
  * https://serverfault.com/questions/138427/what-does-virtual-memory-size-in-top-mean
  * https://elinux.org/images/4/4c/Ott.pdf
</b></details>

<details>
<summary>What is a swap space?</summary><br><b>
  
Explanation: https://itsfoss.com/create-swap-file-linux/
</b></details>

<details>
<summary>What is zombie process?</summary><br><b>
Explanation: 
  
  * https://en.wikipedia.org/wiki/Zombie_process
  * https://www.geeksforgeeks.org/zombie-processes-prevention/
  * https://stackoverflow.com/questions/16944886/how-to-kill-zombie-process
</b></details>

<details>
<summary>File types in Linux</summary><br><b>
Explanation:
  https://www.linux.com/tutorials/file-types-linuxunix-explained-detail/
</b></details>

<details>
<summary> What is proc filesystem?</summary><br><b>
Explanation: 
  
  http://man7.org/linux/man-pages/man5/proc.5.html
</b></details>

<details>
<summary>Linux Process Monitor(TOP). Explain all information from top</summary><br><b>
Explanation: 
  
  https://www.maketecheasier.com/linux-top-explained/
</b></details>

<details>
<summary>What is the difference between hardlinks and symlinks?</summary><br><b>
Explanation: 
  
  https://medium.com/@307/hard-links-and-symbolic-links-a-comparison-7f2b56864cdd
</b></details>

<details>
<summary>What happens if you delete the root user?</summary><br><b>
Explanation: 
  
  * In most cases you will get unbootable system
  * https://askubuntu.com/questions/962660/what-happens-if-you-delete-the-root-user
</b></details>

<details>
<summary>What is a chroot?</summary><br><b>
Explanation: 
  
  https://www.howtogeek.com/441534/how-to-use-the-chroot-command-on-linux/
</b></details>

<details>
<summary>What is OOM and OOMkiller? How it OOM killer is working</summary><br><b>
Explanation:
  
  * https://dev.to/rrampage/surviving-the-linux-oom-killer-2ki9
  * https://www.percona.com/blog/2019/08/02/out-of-memory-killer-or-savior/
</b></details>

<details>
<summary>What is kernel panic?</summary><br><b>
Explanation: 
  
  * https://www.linuxjournal.com/content/oops-debugging-kernel-panics-0
  * http://www.linuxandubuntu.com/home/things-to-know-about-linux-kernel-panic
</b></details>

<details>
<summary>What is 'nohup' used for?</summary><br><b>
Explanation: 
  
  https://www.computerhope.com/unix/unohup.htm
</b></details>

<details>
<summary> What can you do to restore deleted bash script(script is running but deleted by error)?</summary><br><b>
Explanation: 
  
  See filesystem /proc and find ID proccess in that directory should be script
</b></details>

<details>
<summary> What is RAID?</summary><br><b>
Explanation: 
  
  https://en.wikipedia.org/wiki/Standard_RAID_levels
</b></details>

<details>
<summary>What happens when a hardlink is removed?</summary><br><b>
Explanation: 
  
  The file will be deleted if you delete only the last hardlink to this file. 
</b></details>

<details>
<summary>Imagine you executed command `chmod -x /bin/chmod`. How to fix this? </summary><br><b>
Explanation: 
  
  Solution1:
  ```
  cp /bin/cp /tmp/chmod
  cp /bin/chmod /tmp/chmod
  ./tmp/chmod 755 /bin/chmod
  
  ```
  
  Solution2:
  ```
  perl -e 'chmod(0755, "chmod")`
  
  ```
  
  Solution3:
  ```
 /lib/ld-linux.so.2 /bin/chmod 755 /bin/chmod
 
 ```
  
</b></details>

<details>
<summary>What is Load Average?</summary><br><b>
Explanation: 
  
  http://www.brendangregg.com/blog/2017-08-08/linux-load-averages.html
</b></details>

<details>
<summary>What are cgroups?</summary><br><b>
Explanation:
  
  https://www.linuxjournal.com/content/everything-you-need-know-about-linux-containers-part-i-linux-control-groups-and-process
</b></details>

## Networking and Security

<details>
<summary>What is NAT?</summary><br><b>
Explanation: 
  
  * https://www.geeksforgeeks.org/network-address-translation-nat/
  * https://www.comptia.org/content/guides/what-is-network-address-translation
</b></details>

<details>
<summary>What is VLAN?</summary><br><b>
Explanation:
  
  https://study-ccna.com/what-is-a-vlan/
</b></details>

<details>
<summary>What is ARP?</summary><br><b>
Explanation: 
  
  Address Resolution Protocol. 
  https://en.wikipedia.org/wiki/Address_Resolution_Protocol
</b></details>

<details>
<summary> How many layers are there under TCP/IP? Compare OSI and TCP/IP</summary><br><b>
Explanation: 
  
  https://techdifferences.com/difference-between-tcp-ip-and-osi-model.html
</b></details>

<details>
<summary>EXplain TCP 3-way handshake proccess</summary><br><b>
Explanation: 
  
  https://www.geeksforgeeks.org/tcp-3-way-handshake-process/
</b></details>

<details>
<summary>What is SSH and how does it work?</summary><br><b>
Explanation:
  
  https://www.ssh.com/ssh/command
</b></details>

<details>
<summary>Explain DNS records: SOA, PTR, A, MX, and CNAME</summary><br><b>
Explanation: 
  
  https://www.presslabs.com/how-to/dns-records/
</b></details>

<details>
<summary>How to check route table in Linux?</summary><br><b>
Explanation: 
  
  `netstat -rn`
  
  `route -n`
  
  `ip route list`
</b></details>

<details>
<summary>Server1 can't reach to Server2. Describe possible reasons</summary><br><b>
Explanation: 
  
  * Application layer: 
    Check if servers are correctly configured and services up and running
  * Transport layer:
    Check ports, check ping from server to server
  * Network layer:
    Check firewall and networking setting. Also check routes, dns and ARP tables.
</b></details>

<details>
<summary>How to check all of open ports on server?</summary><br><b>
Explanation:
  
  * nmap - if you need check all ports for remote server
  * netstat - for localhost
</b></details>



## Programming

### BASH

<details>
<summary>How to check if the previous command was run successfully?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is function? How to write a function?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>Loops in BASH</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary> How would you compare the strings in a bash script?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary> How to print all array elements and their indexes?</summary><br><b>
Explanation:
  
  ```  
  #!/bin/sh
  array=("A" "B" "C" "X" )
  echo ${array[0]} 
  
  ```
 
</b></details>


<details>
<summary>How to debug a shell script ?</summary><br><b>
Explanation:
  
  Option `-x`
  or `-nv`
</b></details>


### Python
<details>
<summary>Python for sysadmins</summary><br><b>
Explanation:
  
  * https://realpython.com/
  * https://python-for-system-administrators.readthedocs.io/en/latest/
</b></details>

## Databases

<details>
<summary>What is SQL?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>SQL vs NoSQL. Explain benefits of both</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What are tables and field?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is an index?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is primary key?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is database recplication?</summary><br><b>
Explanation: 
  TODO
</b></details>

## Version Control System (GIT) 

<details>
<summary>What is GIT?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary> What are the benefits of using GIT?</summary><br><b>
Explanation:
  TODO
</b></details>

<details>
<summary>What is the difference between `git pull` and `git fetch` ?</summary><br><b>
Explanation:
  TODO
</b></details>

<details>
<summary>What is the difference between `git reset` and `git revert` ?</summary><br><b>
Explanation:
  TODO
</b></details>

<details>
<summary>What is `git rebase` ?</summary><br><b>
Explanation:
  TODO
</b></details>

<details>
<summary>How to reset last commit?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>Describe a dev/test/production workflow using GIT</summary><br><b>
Explanation: 
  TODO
</b></details>

## Containers

<details>
<summary>What is LXC?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is Docker?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What are the advantages of using Docker container?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>Docker RUN vs CMD vs ENTRYPOINT</summary><br><b>
Explanation:
  
  https://goinbigdata.com/docker-run-vs-cmd-vs-entrypoint/
</b></details>

<details>
<summary>What is the difference between ADD and COPY in Dockerfile?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is Docker registry?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is Docker volume?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is docker namespaces?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is docker multistage build? Create one example</summary><br><b>
Explanation: 
  TODO
</b></details>

## Kubernetes

<details>
<summary>Why we need container orchestration?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is kubernetes?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What are the features of Kubernetes?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is POD?</summary><br><b>
Explanation:
  TODO
</b></details>

<details>
<summary>What is kubelet?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is kubectl?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is CNI?</summary><br><b>
Explanation:
  TODO
</b></details>

<details>
<summary>What is headless service?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What are the units of CPU and memory in POD definition?</summary><br><b>
Explanation: 
  
  * CPU is in milicores and memory in bytes
  * https://www.noqcks.io/notes/2018/02/03/understanding-kubernetes-resources/
</b></details>

<details>
<summary>How to deploy stateful application in Kubernetes?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>How to expose Kubernetes service?</summary><br><b>
Explanation: 
  TODO
</b></details>

## DEVOPS

### Config management 

<details>
<summary>Ansible tutorials</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>Salt tutorials</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>Puppet tutorials</summary><br><b>
Explanation: 
  TODO
</b></details>

### CI/CD

<details>
<summary>What is continuous integration?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is continuous delivery?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What is continuous deployment?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>What are the benefits of CI/CD?</summary><br><b>
Explanation: 
  TODO
</b></details>

<details>
<summary>Describe a simple CI/CD Pipeline</summary><br><b>
Explanation: 
  
  https://semaphoreci.com/cicd
  https://www.redhat.com/en/topics/devops/what-is-ci-cd
</b></details>

<details>
<summary>Describe deployment strategies</summary><br><b>
Explanation: 
  
  https://thenewstack.io/deployment-strategies
</b></details>

<details>
<summary>Jenkins tutorials</summary><br><b>
Explanation: 
  
  https://www.udemy.com/share/101WuI/
  https://www.youtube.com/playlist?list=PL9ooVrP1hQOGM6eCsjnfAousUSvpqD8dW&ref=hackr.io
  https://jenkins.io/doc/book/
  
</b></details>


### Infrastructure as code 

<details>
<summary>Terraform</summary><br><b>
Explanation: 
  
  http://www.itkitchen.net/k8s-in-gke-with-terraform/
  https://www.youtube.com/watch?v=TFLQcgZr0no
  https://www.udemy.com/share/101ZdI/
</b></details>



### Clouds

<details>
<summary>What is PaaS, SaaS, IaaS?</summary><br><b>
Explanation: 
 
 TODO
</b></details>


<details>
<summary>What is private cloud?</summary><br><b>
Explanation: 
 
 TODO
</b></details>

<details>
<summary>What is public cloud?</summary><br><b>
Explanation: 
 
 TODO
</b></details>

<details>
<summary>What is cloud service?</summary><br><b>
Explanation: 
 
 TODO
</b></details>

<details>
<summary>What is serverless service?</summary><br><b>
Explanation: 
 
 TODO
</b></details>

<details>
<summary>AWS tutorials</summary><br><b>
Explanation: 
 
 TODO
</b></details>

<details>
<summary>Google Cloud tutorials</summary><br><b>
Explanation: 
 
 TODO
</b></details>

<details>
<summary>Openstack tutorials</summary><br><b>
Explanation: 
  
  The best resource with Openstack cources is LinuxAcademy
  https://linuxacademy.com/library/search/openstack/
</b></details>

## Books and courses

* Brendan Gregg http://www.brendangregg.com/blog/index.html
* Systems Performance http://www.brendangregg.com/sysperfbook.html
* The Phoenix project https://www.amazon.com/Phoenix-Project-DevOps-Helping-Business/dp/1942788290/
* SRE https://landing.google.com/sre/books/
* Linux System Administration Handbook 5th by Evi Nemeth
* The DevOps Handbook: How to Create World-Class Agility, Reliability, and Security in Technology Organizations



