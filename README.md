# ansible-role-vscode

![Ansible](https://github.com/avnes/ansible-role-vscode/actions/workflows/pr-validator.yaml/badge.svg)

Ansible role for installing Visual Studio Code with extensions and configuring it with a slightly opinionated configuration.

# :warning: Repository not maintained :warning:

Please note that this repository is currently archived, and is no longer being maintained.

- It may contain code, or reference dependencies, with known vulnerabilities
- It may contain out-dated advice, how-to's or other forms of documentation

The contents might still serve as a source of inspiration, but please review any contents before reusing elsewhere.

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
