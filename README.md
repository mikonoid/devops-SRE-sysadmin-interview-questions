# Devops/SRE interview preparation questions
This repo is agregated guide for preparation to Devops/SRE engineer interview
#### If you want to thank the author https://www.buymeacoffee.com/mikonoid

## Linux

<details>
<summary>History of OS</summary><br><b>
Explanation: https://www.geeksforgeeks.org/evolution-of-operating-system/
</b></details>

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
  https://docs.kernel.org/filesystems/proc.html
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
<summary>How to check if the last command was run successfully?</summary><br><b>
Explanation:

  `echo $?` if returns 0 that last command executed successfully

</b></details>

<details>
<summary>What is function? How to write a function?</summary><br><b>
Explanation:

  https://linuxize.com/post/bash-functions/
</b></details>

<details>
<summary>Loops in BASH</summary><br><b>
Explanation:

  https://www.tldp.org/HOWTO/Bash-Prog-Intro-HOWTO-7.html
</b></details>

<details>
<summary> How would you compare two strings in a bash script?</summary><br><b>
Explanation:
  Case1:

  ```
  #!/bin/bash

VAR1="string1"
VAR2="string333"

if [ "$VAR1" = "$VAR2" ]; then
    echo "Strings are equal."
else
    echo "Strings are not equal."
fi
```
  Case2:

  ```
  [[ "string1" == "string2" ]] && echo "Equal" || echo "Not equal"

```

</b></details>

<details>
<summary> How to print all array elements and their indexes?</summary><br><b>
Explanation:

  ```
  #!/bin/bash
  array=("A" "B" "C" "X" )
  echo ${array[0]}

  ```

</b></details>

<details>
<summary>Print number from 1 to 10 using for loop</summary><br><b>
Explanation:

  ```
  #!/bin/bash
  for i in {1..10}; do
      echo $i
  done

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

<details>
<summary>How to compile python application?</summary><br><b>
Explanation:

  There are two ways could go about to solve that problem:

* Use a static builder, like freeze, or pyinstaller, or py2exe
* Compile using cython
</b></details>


<details>
<summary>What is PEP 8 and why is it important?</summary><br><b>
Explanation:

  * https://realpython.com/python-pep8/

</b></details>

## Databases

<details>
<summary>What is SQL?</summary><br><b>
Explanation:
  * http://www.sqlcourse.com/intro.html
</b></details>

<details>
<summary>SQL vs NoSQL. Explain benefits of both</summary><br><b>
Explanation:

  * https://www.youtube.com/watch?v=ZS_kXvOeQ5Y
  * https://www.geeksforgeeks.org/difference-between-sql-and-nosql/
</b></details>

<details>
<summary>What are tables and field?</summary><br><b>
Explanation:

  * https://intellipaat.com/blog/tutorial/sql-tutorial/tables-in-sql/
</b></details>

<details>
<summary>What is an index?</summary><br><b>
Explanation:
  * https://www.tutorialspoint.com/sql/sql-indexes.htm
</b></details>

<details>
<summary>What is primary key?</summary><br><b>
Explanation:
  * https://www.w3schools.com/sql/sql_primarykey.ASP
</b></details>

<details>
<summary>What is database recplication?</summary><br><b>
Explanation:

  * https://www.geeksforgeeks.org/data-replication-in-dbms/
</b></details>

<details>
<summary>What is DynamoDB?</summary><br><b>
Explanation:

  * https://www.dynamodbguide.com/what-is-dynamo-db/
</b></details>

## Version Control System (GIT)

<details>
<summary>What is GIT?</summary><br><b>
Explanation:

  * https://git-scm.com/book/en/v2/Getting-Started-What-is-Git
  * https://git-scm.com/book/en/v2/Getting-Started-What-is-Git

</b></details>

<details>
<summary> What are the benefits of using GIT?</summary><br><b>
Explanation:

  * Documentation
  * Markdown
  * Fully Distributed
  * Simplicity
  * Branching model
  * open source

</b></details>

<details>
<summary>What is the difference between `git pull` and `git fetch` ?</summary><br><b>
Explanation:

  * https://guide.freecodecamp.org/miscellaneous/git-pull-vs-git-fetch/

</b></details>

<details>
<summary>What is the difference between `git reset` and `git revert` ?</summary><br><b>
Explanation:

  * https://stackoverflow.com/questions/8358035/whats-the-difference-between-git-revert-checkout-and-reset

</b></details>

<details>
<summary>What is `git rebase` ?</summary><br><b>
Explanation:

  * https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase

</b></details>

<details>
<summary>How to reset last commit?</summary><br><b>
Explanation:

 * `git reset --hard HEAD~1` - not a true way cuz you will lost all changes
 * `git revert <commit-id>` - good way

 for more https://stackoverflow.com/questions/927358/how-do-i-undo-the-most-recent-local-commits-in-git

</b></details>

<details>
<summary>Describe a dev/test/production workflow using GIT</summary><br><b>
Explanation:

  * https://medium.com/@patrickporto/4-branching-workflows-for-git-30d0aaee7bf
  * https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow

</b></details>


## DEVOPS

### Config management

<details>
<summary>Ansible tutorials</summary><br><b>
Explanation:

  * Ansible for Devops https://leanpub.com/ansible-for-devops
  * https://serversforhackers.com/c/an-ansible-tutorial
  * https://medium.com/quick-code/top-tutorials-to-learn-ansible-33afd23ea160
</b></details>

<details>
<summary>Salt tutorials</summary><br><b>
Explanation:

  * https://docs.saltstack.com/en/master/topics/tutorials/walkthrough.html
  * https://www.digitalocean.com/community/tutorials/an-introduction-to-saltstack-terminology-and-concepts
</b></details>

<details>
<summary>Puppet tutorials</summary><br><b>
Explanation:

  * https://www.guru99.com/puppet-tutorial.html
</b></details>

### CI/CD

<details>
<summary>What is continuous integration?</summary><br><b>
Explanation:

  * https://www.youtube.com/watch?v=_zCyLT33moA
  * https://www.atlassian.com/continuous-delivery/continuous-integration
</b></details>

<details>
<summary>What is continuous delivery?</summary><br><b>
Explanation:

  * https://www.atlassian.com/continuous-delivery/principles/continuous-integration-vs-delivery-vs-deployment
  * https://aws.amazon.com/devops/continuous-delivery/
</b></details>

<details>
<summary>What is continuous deployment?</summary><br><b>
Explanation:

  * https://www.atlassian.com/continuous-delivery/continuous-deployment
</b></details>

<details>
<summary>What are the benefits of CI/CD?</summary><br><b>
Explanation:

  * https://www.katalon.com/resources-center/blog/benefits-continuous-integration-delivery/
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

  * https://www.udemy.com/share/101WuI/
  * https://www.youtube.com/playlist?list=PL9ooVrP1hQOGM6eCsjnfAousUSvpqD8dW&ref=hackr.io
  * https://jenkins.io/doc/book/

</b></details>

<details>
<summary>K8S native CI/CD</summary><br><b>
Explanation:

  * Tekton https://github.com/tektoncd
  * ArgoCD https://argoproj.github.io/argo-cd/
  * JenkinsX https://jenkins-x.io/


</b></details>

### Containerization & Orchestration

<details>
<summary>What is a container? How does it differ from a VM?</summary><br><b>
Explanation:

  * https://www.docker.com/resources/what-container
  * https://www.backblaze.com/blog/vm-vs-containers/
</b></details>

<details>
<summary>What is Docker?</summary><br><b>
Explanation:

  * https://docs.docker.com/get-started/overview/
  * https://www.redhat.com/en/topics/containers/what-is-docker
</b></details>

<details>
<summary>Explain Docker architecture</summary><br><b>
Explanation:

  * Docker daemon, Docker client, Docker registry
  * https://docs.docker.com/get-started/overview/#docker-architecture
</b></details>

<details>
<summary>What is the difference between Docker image and container?</summary><br><b>
Explanation:

  * Image is a template, container is a running instance
  * https://stackoverflow.com/questions/23735149/what-is-the-difference-between-a-docker-image-and-a-container
</b></details>

<details>
<summary>What is Dockerfile? Explain best practices</summary><br><b>
Explanation:

  * https://docs.docker.com/engine/reference/builder/
  * https://docs.docker.com/develop/dev-best-practices/
</b></details>

<details>
<summary>What is Docker Compose?</summary><br><b>
Explanation:

  * https://docs.docker.com/compose/
</b></details>

<details>
<summary>Docker multi-stage builds</summary><br><b>
Explanation:

  * https://docs.docker.com/build/building/multi-stage/
</b></details>

<details>
<summary>Docker RUN vs CMD vs ENTRYPOINT</summary><br><b>
Explanation:

  * https://goinbigdata.com/docker-run-vs-cmd-vs-entrypoint/
</b></details>

<details>
<summary>What is the difference between ADD and COPY in Dockerfile?</summary><br><b>
Explanation:

  * https://dev.to/lasatadevi/docker-cmd-vs-entrypoint-34e0
</b></details>

<details>
<summary>What is Docker registry?</summary><br><b>
Explanation:

  * https://docs.docker.com/registry/
  * Storage for docker images
</b></details>

<details>
<summary>What is Docker volume?</summary><br><b>
Explanation:

  * https://docs.docker.com/storage/volumes/
</b></details>

<details>
<summary>What is docker namespaces?</summary><br><b>
Explanation:

  * https://success.docker.com/article/introduction-to-user-namespaces-in-docker-engine
</b></details>

<details>
<summary>History of containers (LXC, chroot)</summary><br><b>
Explanation:

  * https://www.aquasec.com/blog/a-brief-history-of-containers-from-1970s-chroot-to-docker-2016/
  * https://linuxcontainers.org/lxc/introduction/
</b></details>

<details>
<summary>What is Kubernetes?</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/
  * Kubernetes in 5 minutes: https://www.youtube.com/watch?v=PH-2FfFD2PU
</b></details>

<details>
<summary>Why we need container orchestration?</summary><br><b>
Explanation:

  * https://opensource.com/life/16/9/containing-container-chaos-kubernetes
</b></details>

<details>
<summary>Kubernetes architecture (Control Plane, Worker Nodes)</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/architecture/
</b></details>

<details>
<summary>What are Kubernetes pods, deployments, services, ingress?</summary><br><b>
Explanation:

  * Pods: https://kubernetes.io/docs/concepts/workloads/pods/
  * Deployments: https://kubernetes.io/docs/concepts/workloads/controllers/deployment/
  * Services: https://kubernetes.io/docs/concepts/services-networking/service/
  * Ingress: https://kubernetes.io/docs/concepts/services-networking/ingress/
</b></details>

<details>
<summary>What is a namespace in Kubernetes?</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/
</b></details>

<details>
<summary>ConfigMaps and Secrets in Kubernetes</summary><br><b>
Explanation:

  * ConfigMaps: https://kubernetes.io/docs/concepts/configuration/configmap/
  * Secrets: https://kubernetes.io/docs/concepts/configuration/secret/
</b></details>

<details>
<summary>What are StatefulSets and when to use them?</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/
</b></details>

<details>
<summary>What is a DaemonSet?</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/
</b></details>

<details>
<summary>Kubernetes persistent volumes and storage classes</summary><br><b>
Explanation:

  * PV: https://kubernetes.io/docs/concepts/storage/persistent-volumes/
  * Storage Classes: https://kubernetes.io/docs/concepts/storage/storage-classes/
</b></details>

<details>
<summary>What is Helm?</summary><br><b>
Explanation:

  * https://helm.sh/docs/
  * https://www.redhat.com/en/topics/devops/what-is-helm
</b></details>

<details>
<summary>Kubernetes resource limits and requests</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
</b></details>

<details>
<summary>Kubernetes networking model</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/cluster-administration/networking/
</b></details>

<details>
<summary>What are init containers?</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/workloads/pods/init-containers/
</b></details>

<details>
<summary>Kubernetes probes (liveness, readiness, startup)</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/
</b></details>

<details>
<summary>What is kubelet?</summary><br><b>
Explanation:

  * Kubelet - agent on a kubernetes cluster's node that takes care of all activity on that node
  * https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet/
</b></details>

<details>
<summary>What is kubectl?</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/reference/kubectl/overview/
</b></details>

<details>
<summary>What is CNI (Container Network Interface)?</summary><br><b>
Explanation:

  * https://www.dasblinkenlichten.com/understanding-cni-container-networking-interface/
</b></details>

<details>
<summary>What is headless service?</summary><br><b>
Explanation:

  * https://dev.to/kaoskater08/building-a-headless-service-in-kubernetes-3bk8
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

  * https://cloud.google.com/kubernetes-engine/docs/how-to/stateful-apps
  * https://kubernetes.io/docs/tasks/run-application/run-replicated-stateful-application/
</b></details>

<details>
<summary>Kubernetes deployment strategies: blue-green, canary, rolling</summary><br><b>
Explanation:

  * https://traefik.io/glossary/kubernetes-deployment-strategies-blue-green-canary/
</b></details>

<details>
<summary>Kubernetes etcd - how to backup etcd</summary><br><b>
Explanation:

  * https://medium.com/@mehmetodabashi/backup-and-restore-etcd-cluster-on-kubernetes-93c19b1c070
  * https://kubernetes.io/docs/tasks/administer-cluster/configure-upgrade-etcd/
</b></details>

<details>
<summary>Custom Resource Definitions (CRD)</summary><br><b>
Explanation:

  * https://spacelift.io/blog/kubernetes-crd
  * https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/
</b></details>

<details>
<summary>NodePort vs ClusterIP</summary><br><b>
Explanation:

  * https://edgedelta.com/company/blog/kubernetes-services-types
  * https://kubernetes.io/docs/tutorials/kubernetes-basics/expose/expose-intro/
</b></details>

### Monitoring & Logging

<details>
<summary>What is observability?</summary><br><b>
Explanation:

  * https://www.ibm.com/cloud/learn/observability
  * Three pillars: metrics, logs, traces
</b></details>

<details>
<summary>What is Prometheus?</summary><br><b>
Explanation:

  * https://prometheus.io/docs/introduction/overview/
</b></details>

<details>
<summary>Prometheus architecture and components</summary><br><b>
Explanation:

  * https://prometheus.io/docs/introduction/overview/#architecture
</b></details>

<details>
<summary>What is Grafana?</summary><br><b>
Explanation:

  * https://grafana.com/docs/grafana/latest/introduction/
</b></details>

<details>
<summary>ELK Stack (Elasticsearch, Logstash, Kibana)</summary><br><b>
Explanation:

  * https://www.elastic.co/what-is/elk-stack
</b></details>

<details>
<summary>What is distributed tracing? Jaeger, Zipkin</summary><br><b>
Explanation:

  * https://opentelemetry.io/docs/concepts/observability-primer/#distributed-traces
  * Jaeger: https://www.jaegertracing.io/
  * Zipkin: https://zipkin.io/
</b></details>

<details>
<summary>Log aggregation vs log streaming</summary><br><b>
Explanation:

  * Fluentd, Fluent Bit, Logstash comparison
  * https://logz.io/blog/fluentd-logstash/
</b></details>

<details>
<summary>What are SLI, SLO, SLA?</summary><br><b>
Explanation:

  * https://cloud.google.com/blog/products/devops-sre/sre-fundamentals-slis-slas-and-slos
  * https://sre.google/sre-book/service-level-objectives/
</b></details>

<details>
<summary>What is APM (Application Performance Monitoring)?</summary><br><b>
Explanation:

  * https://www.dynatrace.com/news/blog/what-is-apm-2/
  * Tools: New Relic, Datadog, Dynatrace
</b></details>

### GitOps

<details>
<summary>What is GitOps?</summary><br><b>
Explanation:

  * https://www.gitops.tech/
  * https://www.weave.works/technologies/gitops/
</b></details>

<details>
<summary>GitOps tools (ArgoCD, Flux)</summary><br><b>
Explanation:

  * ArgoCD: https://argo-cd.readthedocs.io/en/stable/
  * Flux: https://fluxcd.io/
</b></details>

### Security & Compliance

<details>
<summary>What is DevSecOps?</summary><br><b>
Explanation:

  * https://www.redhat.com/en/topics/devops/what-is-devsecops
</b></details>

<details>
<summary>Container security scanning (Trivy, Clair, Aqua)</summary><br><b>
Explanation:

  * Trivy: https://github.com/aquasecurity/trivy
  * https://sysdig.com/learn-cloud-native/kubernetes-security/kubernetes-image-scanning/
</b></details>

<details>
<summary>What is SAST and DAST?</summary><br><b>
Explanation:

  * https://www.synopsys.com/glossary/what-is-sast.html
  * https://www.microfocus.com/en-us/what-is/dast
</b></details>

<details>
<summary>Secret management (HashiCorp Vault, AWS Secrets Manager)</summary><br><b>
Explanation:

  * Vault: https://www.vaultproject.io/
  * AWS Secrets Manager: https://aws.amazon.com/secrets-manager/
</b></details>

<details>
<summary>What is RBAC in Kubernetes?</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/reference/access-authn-authz/rbac/
</b></details>

<details>
<summary>What are admission controllers in Kubernetes?</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/
</b></details>

<details>
<summary>Network policies in Kubernetes</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/services-networking/network-policies/
</b></details>

<details>
<summary>What is Pod Security Policy/Pod Security Standards?</summary><br><b>
Explanation:

  * https://kubernetes.io/docs/concepts/security/pod-security-standards/
</b></details>

### Version Control & Collaboration

<details>
<summary>Git branching strategies (GitFlow, trunk-based)</summary><br><b>
Explanation:

  * https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow
  * https://trunkbaseddevelopment.com/
</b></details>

<details>
<summary>What is monorepo vs polyrepo?</summary><br><b>
Explanation:

  * https://www.atlassian.com/git/tutorials/monorepos
</b></details>

<details>
<summary>Code review best practices</summary><br><b>
Explanation:

  * https://google.github.io/eng-practices/review/
</b></details>

### Service Mesh

<details>
<summary>What is a service mesh?</summary><br><b>
Explanation:

  * https://www.redhat.com/en/topics/microservices/what-is-a-service-mesh
</b></details>

<details>
<summary>Istio overview</summary><br><b>
Explanation:

  * https://istio.io/latest/docs/concepts/what-is-istio/
</b></details>

<details>
<summary>Linkerd overview</summary><br><b>
Explanation:

  * https://linkerd.io/
</b></details>

### Chaos Engineering

<details>
<summary>What is Chaos Engineering?</summary><br><b>
Explanation:

  * https://principlesofchaos.org/
  * https://www.gremlin.com/community/tutorials/chaos-engineering-the-history-principles-and-practice/
</b></details>

<details>
<summary>Chaos Engineering tools (Chaos Monkey, Gremlin, Litmus)</summary><br><b>
Explanation:

  * Chaos Monkey: https://netflix.github.io/chaosmonkey/
  * Gremlin: https://www.gremlin.com/
  * Litmus: https://litmuschaos.io/
</b></details>

### Infrastructure as code

#### Terraform questions

<details>
<summary>Terraform tutorials</summary><br><b>
Explanation:

  * https://www.youtube.com/watch?v=TFLQcgZr0no
  * https://www.udemy.com/share/101ZdI/
  * https://itnext.io/terraform-tutorial-part-1-intro-and-basic-concepts-7a27ae7722b6

</b></details>

<details>
<summary>What is terraform modules?</summary><br><b>
Explanation:

  * https://www.freecodecamp.org/news/terraform-modules-explained/

</b></details>

<details>
<summary>What is ".terraform" directory?</summary><br><b>
Explanation:

```The ".terraform" directory is a local cache where Terraform retains some files required for subsequent operations against this configuration. Its contents are not intended to be included in version control.```

</b></details>

<details>
<summary>What is the usage of Terraform init?</summary><br><b>
Explanation:

```Terraform init is a command used to initialize the Terraform code. Let's see the all usage of Terraform init command:

* Terraform init command is used to initialize the working directory containing Terraform configuration files.
* It is used for Plugin Installation.
* It is also used for Child Module Installation.
* It is used for Backend Initialization.
* You can safely run this command multiple times.
```

</b></details>

<details>
<summary>What do you understand by Terraform Backends? What are the most recommended Backends we should use?</summary><br><b>
Explanation:

```Terraform backends are used to define where and how operations are performed, where state snapshots are stored, etc. Each Terraform configuration can specify a backend.```

Reference:
* https://developer.hashicorp.com/terraform/language/settings/backends/configuration

</b></details>

<details>
<summary>What is terraform lock file?</summary><br><b>

 Explanation:

* https://developer.hashicorp.com/terraform/language/files/dependency-lock

</b></details>

#### AWS Cloudformation

<details>
<summary>AWS CloudFormation</summary><br><b>

Explanation:

  * https://www.youtube.com/watch?v=0Sh9OySCyb4
  * https://www.simplilearn.com/tutorials/aws-tutorial/aws-cloudformation

</b></details>



## Clouds

### Cloud Computing Fundamentals

<details>
<summary>What is PaaS, SaaS, IaaS?</summary><br><b>
Explanation:

 * https://www.ibm.com/cloud/learn/iaas-paas-saas
</b></details>

<details>
<summary>What is private cloud?</summary><br><b>
Explanation:

 * https://azure.microsoft.com/en-us/overview/what-are-private-public-hybrid-clouds/
</b></details>

<details>
<summary>What is public cloud?</summary><br><b>
Explanation:

 * https://azure.microsoft.com/en-us/overview/what-is-a-public-cloud/
 * examples: AWS, GCP, DigitalOcean, Azure
</b></details>

<details>
<summary>What is hybrid cloud?</summary><br><b>
Explanation:

 * https://www.ibm.com/cloud/learn/hybrid-cloud
</b></details>

<details>
<summary>What is multi-cloud?</summary><br><b>
Explanation:

 * https://www.redhat.com/en/topics/cloud-computing/what-is-multicloud
</b></details>

<details>
<summary>What is cloud service?</summary><br><b>
Explanation:

 * https://searchitchannel.techtarget.com/definition/cloud-services
</b></details>

<details>
<summary>What is serverless computing?</summary><br><b>
Explanation:

 * https://en.wikipedia.org/wiki/Serverless_computing
 * https://aws.amazon.com/serverless/
</b></details>

<details>
<summary>What is cloud-native?</summary><br><b>
Explanation:

 * https://www.cncf.io/about/faq/
</b></details>

<details>
<summary>What is elasticity in cloud computing?</summary><br><b>
Explanation:

 * Ability to scale resources up or down based on demand
 * https://www.ibm.com/cloud/learn/benefits-of-cloud-computing
</b></details>

<details>
<summary>What is cloud availability zone?</summary><br><b>
Explanation:

 * https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html
</b></details>

<details>
<summary>What is a cloud region?</summary><br><b>
Explanation:

 * Geographic location where cloud provider has data centers
 * https://cloud.google.com/compute/docs/regions-zones
</b></details>

### AWS (Amazon Web Services)

<details>
<summary>AWS tutorials and resources</summary><br><b>
Explanation:

 * https://aws.amazon.com/getting-started/
 * https://docs.aws.amazon.com/
 * https://medium.com/javarevisited/5-best-aws-courses-for-beginners-and-experienced-developers-to-learn-in-2021-563212409fbd
</b></details>

<details>
<summary>What is EC2?</summary><br><b>
Explanation:

 * Elastic Compute Cloud - virtual servers in the cloud
 * https://aws.amazon.com/ec2/
</b></details>

<details>
<summary>What is S3?</summary><br><b>
Explanation:

 * Simple Storage Service - object storage
 * https://aws.amazon.com/s3/
</b></details>

<details>
<summary>What is VPC?</summary><br><b>
Explanation:

 * Virtual Private Cloud - isolated network in AWS
 * https://aws.amazon.com/vpc/
</b></details>

<details>
<summary>What is AWS Lambda?</summary><br><b>
Explanation:

 * Serverless compute service
 * https://aws.amazon.com/lambda/
</b></details>

<details>
<summary>What is RDS?</summary><br><b>
Explanation:

 * Relational Database Service
 * https://aws.amazon.com/rds/
</b></details>

<details>
<summary>What is ECS and EKS?</summary><br><b>
Explanation:

 * ECS - Elastic Container Service
 * EKS - Elastic Kubernetes Service
 * https://aws.amazon.com/ecs/
 * https://aws.amazon.com/eks/
</b></details>

<details>
<summary>What is CloudFormation?</summary><br><b>
Explanation:

 * Infrastructure as Code service
 * https://aws.amazon.com/cloudformation/
 * https://www.simplilearn.com/tutorials/aws-tutorial/aws-cloudformation
</b></details>

<details>
<summary>What is IAM in AWS?</summary><br><b>
Explanation:

 * Identity and Access Management
 * https://aws.amazon.com/iam/
</b></details>

<details>
<summary>What is CloudWatch?</summary><br><b>
Explanation:

 * Monitoring and observability service
 * https://aws.amazon.com/cloudwatch/
</b></details>

<details>
<summary>What is Route53?</summary><br><b>
Explanation:

 * DNS web service
 * https://aws.amazon.com/route53/
</b></details>

<details>
<summary>What is Elastic Load Balancer (ELB)?</summary><br><b>
Explanation:

 * Distributes incoming traffic across multiple targets
 * ALB, NLB, CLB differences
 * https://aws.amazon.com/elasticloadbalancing/
</b></details>

<details>
<summary>What is Auto Scaling in AWS?</summary><br><b>
Explanation:

 * Automatically adjusts compute capacity
 * https://aws.amazon.com/autoscaling/
</b></details>

<details>
<summary>What is CloudFront?</summary><br><b>
Explanation:

 * Content Delivery Network (CDN)
 * https://aws.amazon.com/cloudfront/
</b></details>

<details>
<summary>What is SNS and SQS?</summary><br><b>
Explanation:

 * SNS - Simple Notification Service
 * SQS - Simple Queue Service
 * https://aws.amazon.com/sns/
 * https://aws.amazon.com/sqs/
</b></details>

<details>
<summary>What is AWS KMS?</summary><br><b>
Explanation:

 * Key Management Service - encryption key management
 * https://aws.amazon.com/kms/
</b></details>

<details>
<summary>What is AWS Secrets Manager?</summary><br><b>
Explanation:

 * Manage, retrieve, and rotate credentials
 * https://aws.amazon.com/secrets-manager/
</b></details>

<details>
<summary>What is DynamoDB?</summary><br><b>
Explanation:

 * NoSQL database service
 * https://aws.amazon.com/dynamodb/
 * https://www.dynamodbguide.com/what-is-dynamo-db/
</b></details>

<details>
<summary>What is ElastiCache?</summary><br><b>
Explanation:

 * In-memory caching service (Redis, Memcached)
 * https://aws.amazon.com/elasticache/
</b></details>

<details>
<summary>What is AWS Step Functions?</summary><br><b>
Explanation:

 * Serverless workflow orchestration
 * https://aws.amazon.com/step-functions/
</b></details>

<details>
<summary>What is AWS Organizations?</summary><br><b>
Explanation:

 * Centrally manage multiple AWS accounts
 * https://aws.amazon.com/organizations/
</b></details>

### Azure (Microsoft Azure)

<details>
<summary>Azure tutorials and resources</summary><br><b>
Explanation:

 * https://docs.microsoft.com/en-us/learn/azure/
 * https://azure.microsoft.com/en-us/get-started/
</b></details>

<details>
<summary>What is Azure Virtual Machines?</summary><br><b>
Explanation:

 * IaaS compute service
 * https://azure.microsoft.com/en-us/services/virtual-machines/
</b></details>

<details>
<summary>What is Azure App Service?</summary><br><b>
Explanation:

 * PaaS for web apps
 * https://azure.microsoft.com/en-us/services/app-service/
</b></details>

<details>
<summary>What is Azure Blob Storage?</summary><br><b>
Explanation:

 * Object storage solution
 * https://azure.microsoft.com/en-us/services/storage/blobs/
</b></details>

<details>
<summary>What is Azure Functions?</summary><br><b>
Explanation:

 * Serverless compute service
 * https://azure.microsoft.com/en-us/services/functions/
</b></details>

<details>
<summary>What is Azure AKS (Kubernetes Service)?</summary><br><b>
Explanation:

 * Managed Kubernetes service
 * https://azure.microsoft.com/en-us/services/kubernetes-service/
</b></details>

<details>
<summary>What is Azure Resource Manager (ARM)?</summary><br><b>
Explanation:

 * Deployment and management service
 * https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/overview
</b></details>

<details>
<summary>What is Azure Active Directory?</summary><br><b>
Explanation:

 * Identity and access management
 * https://azure.microsoft.com/en-us/services/active-directory/
</b></details>

<details>
<summary>What is Azure DevOps?</summary><br><b>
Explanation:

 * CI/CD and collaboration tools
 * https://azure.microsoft.com/en-us/services/devops/
</b></details>

<details>
<summary>What is Azure Monitor?</summary><br><b>
Explanation:

 * Monitoring and diagnostics
 * https://azure.microsoft.com/en-us/services/monitor/
</b></details>

<details>
<summary>What is Azure SQL Database?</summary><br><b>
Explanation:

 * Managed relational database
 * https://azure.microsoft.com/en-us/services/sql-database/
</b></details>

<details>
<summary>What is Azure Cosmos DB?</summary><br><b>
Explanation:

 * Globally distributed NoSQL database
 * https://azure.microsoft.com/en-us/services/cosmos-db/
</b></details>

<details>
<summary>What is Azure Key Vault?</summary><br><b>
Explanation:

 * Secrets management service
 * https://azure.microsoft.com/en-us/services/key-vault/
</b></details>

<details>
<summary>What is Azure Load Balancer?</summary><br><b>
Explanation:

 * Layer 4 load balancing
 * https://azure.microsoft.com/en-us/services/load-balancer/
</b></details>

<details>
<summary>What is Azure CDN?</summary><br><b>
Explanation:

 * Content Delivery Network
 * https://azure.microsoft.com/en-us/services/cdn/
</b></details>

### GCP (Google Cloud Platform)

<details>
<summary>GCP tutorials and resources</summary><br><b>
Explanation:

 * https://cloud.google.com/training
 * https://www.udemy.com/topic/google-cloud/
 * https://cloud.google.com/docs
</b></details>

<details>
<summary>What is Compute Engine?</summary><br><b>
Explanation:

 * Virtual machines in GCP
 * https://cloud.google.com/compute
</b></details>

<details>
<summary>What is Google Cloud Storage?</summary><br><b>
Explanation:

 * Object storage service
 * https://cloud.google.com/storage
</b></details>

<details>
<summary>What is Cloud Functions?</summary><br><b>
Explanation:

 * Serverless execution environment
 * https://cloud.google.com/functions
</b></details>

<details>
<summary>What is GKE (Google Kubernetes Engine)?</summary><br><b>
Explanation:

 * Managed Kubernetes service
 * https://cloud.google.com/kubernetes-engine
</b></details>

<details>
<summary>What is Cloud Run?</summary><br><b>
Explanation:

 * Fully managed serverless platform for containers
 * https://cloud.google.com/run
</b></details>

<details>
<summary>What is BigQuery?</summary><br><b>
Explanation:

 * Serverless data warehouse
 * https://cloud.google.com/bigquery
</b></details>

<details>
<summary>What is Cloud SQL?</summary><br><b>
Explanation:

 * Managed relational database
 * https://cloud.google.com/sql
</b></details>

<details>
<summary>What is Cloud Spanner?</summary><br><b>
Explanation:

 * Horizontally scalable relational database
 * https://cloud.google.com/spanner
</b></details>

<details>
<summary>What is Firestore?</summary><br><b>
Explanation:

 * NoSQL document database
 * https://cloud.google.com/firestore
</b></details>

<details>
<summary>What is Cloud Pub/Sub?</summary><br><b>
Explanation:

 * Messaging and event ingestion
 * https://cloud.google.com/pubsub
</b></details>

<details>
<summary>What is Cloud IAM?</summary><br><b>
Explanation:

 * Identity and Access Management
 * https://cloud.google.com/iam
</b></details>

<details>
<summary>What is Cloud Monitoring (formerly Stackdriver)?</summary><br><b>
Explanation:

 * Monitoring, logging, and diagnostics
 * https://cloud.google.com/monitoring
</b></details>

<details>
<summary>What is Cloud Load Balancing?</summary><br><b>
Explanation:

 * Distribute traffic across instances
 * https://cloud.google.com/load-balancing
</b></details>

<details>
<summary>What is Cloud CDN?</summary><br><b>
Explanation:

 * Content Delivery Network
 * https://cloud.google.com/cdn
</b></details>

<details>
<summary>What is VPC in GCP?</summary><br><b>
Explanation:

 * Virtual Private Cloud networking
 * https://cloud.google.com/vpc
</b></details>

<details>
<summary>What is Cloud Build?</summary><br><b>
Explanation:

 * CI/CD platform
 * https://cloud.google.com/build
</b></details>

<details>
<summary>What is Anthos?</summary><br><b>
Explanation:

 * Hybrid and multi-cloud application platform
 * https://cloud.google.com/anthos
</b></details>

### Other Cloud Providers

<details>
<summary>What is DigitalOcean?</summary><br><b>
Explanation:

 * Developer-friendly cloud platform
 * https://www.digitalocean.com/
</b></details>

<details>
<summary>OpenStack tutorials</summary><br><b>
Explanation:

 * Open-source cloud computing platform
 * https://www.openstack.org/
 * https://docs.openstack.org/
</b></details>

## Books and courses

* Brendan Gregg http://www.brendangregg.com/blog/index.html
* Systems Performance http://www.brendangregg.com/sysperfbook.html
* The Phoenix project https://www.amazon.com/Phoenix-Project-DevOps-Helping-Business/dp/1942788290/
* SRE https://landing.google.com/sre/books/
* Linux System Administration Handbook 5th by Evi Nemeth
* The DevOps Handbook: How to Create World-Class Agility, Reliability, and Security in Technology Organizations
* Continuous Delivery: Reliable Software Releases through Build, Test, and Deployment Automation by Jez Humble and David Farley
