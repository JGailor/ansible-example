# ansible-example

This is intended to reify the best practices [found here](http://docs.ansible.com/ansible/playbooks_best_practices.html) into a concrete example.

## Configuring the different environments

```
# staging (whole site)
ansible-playbook site.yml -i staging

# staging (just databases)
ansible-playbook database.yml -i staging

# staging (just job servers)
ansible-playbook jobs.yml -i staging
```

```
# experimental (whole site)
ansible-playbook site.yml -i experimental

# experimental (just databases)
ansible-playbook database.yml -i experimental

# experimental (just job servers)
ansible-playbook jobs.yml -i experimental
```

```
# production (whole site)
ansible-playbook site.yml -i production

# production (just databases)
ansible-playbook database.yml -i production

# production (just job servers)
ansible-playbook jobs.yml -i production
```
