# fail2ban

An Ansible role that installs fail2ban and configures sshd protection on EL 7
or Fedora.


## Role Variables

Available variables and their default values are listed below:

* `fail2ban_ignoreip: 127.0.0.1/8` - fail2ban will not ban a host which matches
  an address in this list


## Example Playbook

```yaml
    ---
    - hosts: all
      roles:
        - { role: ezamriy.fail2ban, fail2ban_ignoreip: '127.0.0.1/8 192.168.0.0/24' }
```


## License

MIT


## Authors

* [Eugene Zamriy](https://github.com/ezamriy)
