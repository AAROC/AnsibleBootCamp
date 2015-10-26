Installing Ansible is described at [the Ansible documentation site](http://docs.ansible.com/ansible/intro_installation.html)

Installing Ansible:

  * CentOS :
```
    yum install git python
    yum groupinstall 'Development Tools'
```
  * Debian :
```
    apt-get install git python build-essential python-pip
```

Now : clone Ansible

```
git clone https://github.com/ansible/ansible --recursive
```

# Things that went wrong

  1. On CentOS we got SSL errors.

# Questions

  1. Does Ansible use virtualenv ? 
