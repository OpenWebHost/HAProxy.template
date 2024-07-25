Crucially important to run if using SELinux on Fedora:
https://serverfault.com/questions/654599/weird-interaction-with-systemctl-with-haproxy-on-centos-7/654684#654684

```
semanage port --add --type http_port_t --proto tcp 8001
semanage port --add --type http_port_t --proto tcp 80
semanage port --add --type http_port_t --proto tcp 3000
```

