3 Servers

> Most of the configuration settings are now wrapped in ansible.cfg

Figure out the free space available in the 3 servers
```
ansible vagrant1 -m shell -a "free -m"  
ansible vagrant2 -m shell -a "free -m"
ansible vagrant3 -m shell -a "free -m"    
```