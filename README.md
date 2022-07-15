# voda-datadog-11thjuly2022

<img src="plan.png">

### datadog revision 

### code share URL 

[code_share](https://codeshare.io/X8XK8E)

### starting docker based agent manually --

```
[root@ashu-vm ~]# docker  start  dd-agent 
dd-agent
[root@ashu-vm ~]# docker  ps
CONTAINER ID   IMAGE                      COMMAND                  CREATED      STATUS                 PORTS                                   NAMES
21da87118bd1   ashuapp:v1                 "/docker-entrypoint.…"   2 days ago   Up 3 hours             0.0.0.0:1122->80/tcp, :::1122->80/tcp   ashuc1
21075cf5f1fd   gcr.io/datadoghq/agent:7   "/bin/entrypoint.sh"     3 days ago   Up 3 hours (healthy)   8125/udp, 8126/tcp                      dd-agent
[root@ashu-vm ~]# 

```

### make these changes for persistent docker based datadog agent auto start

```
[root@ashu-vm ~]# systemctl enable --now  docker 
[root@ashu-vm ~]# docker  update  --restart  always  dd-agent 
dd-agent
[root@ashu-vm ~]# docker  start  dd-agent  
dd-agent
```

### metrics explorer 

<img src="mt.png">






