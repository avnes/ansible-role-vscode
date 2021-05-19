master: [![Build Status](https://travis-ci.org/avnes/ansible-role-vscode.png?branch=master)](https://travis-ci.org/avnes/ansible-role-vscode) develop: [![Build Status](https://travis-ci.org/avnes/ansible-role-vscode.png?branch=develop)](https://travis-ci.org/avnes/ansible-role-vscode)

# ansible-role-vscode

Ansible role for installing Visual Studio Code with extensions and configuring it with a slightly opinionated configuration.

## Requirements

None.

## Role Variables

Have a look at defaults/main.yml for user configurable variables. It will mainly be the list vscode_extensions and the boolean vscode_use_config that you would want to tweak.

## Dependencies

None

## Example Playbook

```yaml
- hosts: localhost
  roles:
     - avnes.vscode
```

## Test

```bash
virtualenv ~/.virtualenv/ansible-role-vscode
source ~/.virtualenv/ansible-role-vscode/bin/activate
pip install -r requirements.txt
molecule test
```

## License

MIT

## Author Information

<https://github.com/avnes/>
