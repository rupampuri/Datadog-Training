# voda-datadog-11thjuly2022

<img src="plan.png">

### Monitoring 

<img src="intro.png">

### Observalibity vs monitoring 

<img src="ob.png">

### pillers of OBservability 

<img src="pl.png">

### datadog introduction 

<img src="datadog.png">

### pricing 

<img src="price.png">

### application Infra 

<img src="appinfra.png">

### planning infro in aws cloud 

### connecting linux vm via ssh 

```
fire@ashutoshhs-MacBook-Air ~ % ssh   ec2-user@184.73.12.243
The authenticity of host '184.73.12.243 (184.73.12.243)' can't be established.
ECDSA key fingerprint is SHA256:8nNOk0DD8ITpko+eOq6cAXWZdFJtxq3rPKoRe5BRoBw.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '184.73.12.243' (ECDSA) to the list of known hosts.
ec2-user@184.73.12.243: Permission denied (publickey,gssapi-keyex,gssapi-with-mic).
fire@ashutoshhs-MacBook-Air ~ % 


```

### give hostname to your VM 

```
[ec2-user@ip-172-31-18-110 ~]$ sudo -i 
[root@ip-172-31-18-110 ~]# whoami
root
[root@ip-172-31-18-110 ~]# hostnamectl set-hostname  ashu-vm 
[root@ip-172-31-18-110 ~]# exit
logout
[ec2-user@ip-172-31-18-110 ~]$ sudo -i
[root@ashu-vm ~]# 
[root@ashu-vm ~]# 


```




