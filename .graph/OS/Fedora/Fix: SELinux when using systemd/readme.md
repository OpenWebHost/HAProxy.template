Crucially important to run if using SELinux on Fedora:
https://serverfault.com/questions/654599/weird-interaction-with-systemctl-with-haproxy-on-centos-7/654684#654684

```
# add Docker backend port to SELinux
semanage port --add --type http_port_t --proto tcp 3000
```

