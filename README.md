# Deploying Kubernetes with Kubeadm

Hardware recommandation:

+ 2Core+ CPU & 4GB RAM
+ 30GB+ disk
+ 64bit Linux OS
+ Access to the INTERNET

Copy inventory/kubernetes.yml.example to inventory/kubernetes.yml and replace IPs.

```
[master]
your_master_ip

[worker]
your_worker1_ip
your_worker2_ip
```

## Initialize your cluster

### CentOS

```bash
$ ansible-playbook -i inventory/kubernetes.yml.example centos_deploy.yml
```
