# AWSCLI Ansible Role

Installs the [AWS Command Line Interface](https://aws.amazon.com/cli/).

*   Creates an _awscli_ directory
*   Downloads, validates and extracts the the `awscli` zip
*   Installs the `awcli` and autocomplete for the current user

## Variables

| Name               | Description                                        | Default Value |
|--------------------|----------------------------------------------------|---------------|
| awscli_base_dir    | The _awscli_ directory will be created here        | ~/tools       |
| awscli_install_dir | The directory where the binaries will be installed | ~/bin         |

## Example Playbook

```yaml
- hosts: localhost
  become: yes
  roles:
    - role: japeoh.awscli
      vars:
        awscli_install_dir: /usr/local/bin
```

## License

GPLv3

##  Development

See [here](https://github.com/japeoh/ansible-role-development) for setup.
