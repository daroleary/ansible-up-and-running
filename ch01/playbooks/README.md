Ping our test server

> Most of the configuration settings are now wrapped in ansible.cfg

```
ansible testserver -m ping 
```

Uptime of the server via command
> Used so often its a default module so no need to specify
```
ansible testserver -m command -a uptime
ansible testserver -a uptime
```

Tail file on server
```
ansible testserver -a "tail /var/log/dmesg" 
```

If we need root access, `become` the root user via -b
```
ansible testserver -b -a "tail /var/log/messages"  
``` 