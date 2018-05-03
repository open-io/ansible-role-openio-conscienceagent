[![Build Status](https://travis-ci.org/open-io/ansible-role-openio-conscienceagent.svg?branch=master)](https://travis-ci.org/open-io/ansible-role-openio-conscienceagent)
# Ansible role `conscienceagent`

An Ansible role for Conscience agent. Specifically, the responsibilities of this role are to:

- install the OpenIO Conscienceagent
- configure the OpenIO Conscienceagent

## Requirements

- Ansible 2.4+

## Role Variables


| Variable   | Default | Comments (type)  |
| :---       | :---    | :---             |
| `openio_conscienceagent_namespace` | `"OPENIO"` | Namespace |
| `openio_conscienceagent_serviceid` | `"0"` | ID in gridinit |

## Dependencies

No dependencies.

## Example Playbook

```yaml
- hosts: all
  gather_facts: true
  become: true
  roles:
    - role: conscienceagent
```


```ini
[all]
node1 ansible_host=192.168.1.173
```

## Contributing

Issues, feature requests, ideas are appreciated and can be posted in the Issues section.

Pull requests are also very welcome.
The best way to submit a PR is by first creating a fork of this Github project, then creating a topic branch for the suggested change and pushing that branch to your own fork.
Github can then easily create a PR based on that branch.

## License

Apache License, Version 2.0

## Contributors

- [Guillaume DELAPORTE](https://github.com/GuillaumeDelaporte)(maintainer)
