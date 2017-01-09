# Ansible role for tools of user

- Setup [ghq](https://github.com/motemen/ghq)
- Setup [peco](https://github.com/peco/peco)

## Requirements

- Debian
- Ubuntu

## Role Variables

- `anyenv_home_dir`: path to user's home directory
- `anyenv_plugins`: repositories of anyenv plugins
- `git_update`: `update` option of [git module](http://docs.ansible.com/git_module.html)
- `git_depth`: `depth` option of [git module](http://docs.ansible.com/git_module.html)
- `rbenv_plugins`: repositories of rbenv plugins

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
