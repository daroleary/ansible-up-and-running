NGINX setup

> Most of the configuration settings are now wrapped in ansible.cfg

Start nginx without TLS enabled
```
ansible-playbook web-notls.yml 
```

Start nginx with TLS enabled
```
ansible-playbook web-tls.yml
```