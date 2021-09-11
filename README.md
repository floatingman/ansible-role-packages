# ansible-role-packages

Install applications on an Arch or Ubuntu based systems via its package manager. Optionally, install an AUR package manager on Arch based systems.

## Test

Run `molecule test` to test this role in a docker container

## Requirements

- Arch Linux or Ubuntu based OS
- Sudo permissions

## Role Variables

- `common`: common packages to be installed
- `arch`: packages to be installed on Arch only
- `debian`: packages to be installed on Debian only
- `aur`: set to true to install an [AUR helper](https://aur.archlinux.org/)

## Dependencies

ansible-role-basic

## Example Playbook

See [converge.yml](https://github.com/Allaman/ansible-role-packages/blob/master/molecule/default/converge.yml)

## License

MIT
