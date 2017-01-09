# Ansible role for tools of user

- Setup [ghq](https://github.com/motemen/ghq)
- Setup [peco](https://github.com/peco/peco)

## Requirements

- Debian
- Ubuntu

## Role Variables

- `tools_download_dir`: download directory
- `tools_bin_dir`: bin directory
- `tools_ghq_linux_amd64`: url and checksum of ghq
- `tools_peco_linux_amd64`: url and checksum of peco

## Dependencies

None.

## Example Playbook

Normal usage:

    ---
    - hosts: all
      become: no
      roles:
      - znz.user-tools

## Example requirements.yml

    - src: https://github.com/znz/ansible-role-user-tools
      version: master
      name: znz.user-tools

## License

MIT License
