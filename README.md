# ansible-role-vscode

![Ansible](https://github.com/avnes/ansible-role-vscode/actions/workflows/ansible.yaml/badge.svg)

Ansible role for installing Visual Studio Code with extensions and configuring it with a slightly opinionated configuration.

## Requirements

Poetry. Install it from <https://python-poetry.org/docs/>

## Role Variables

Have a look at defaults/main.yml for user configurable variables. It will mainly be the list vscode_extensions and the boolean vscode_use_config that you would want to tweak.

## Dependencies

None

## Example Playbook

```yaml
- hosts: localhost
  vars:
    config_owner: 'maya'
  roles:
     - avnes.vscode
```

## For pip compability

```bash
poetry export --dev --output requirements.txt
```

## Test

```bash
poetry install
poetry shell
molecule test
```

## License

MIT

## Author Information

<https://github.com/avnes/>
