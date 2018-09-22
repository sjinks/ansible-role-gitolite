# Ansible Role: gitolite

This role installs `gitolite` — a tool to host Git repositories

## Requirements

None.

## Role Variables

  * `gitolite_user`: the user under which gitolite operates (default: `gitolite`)
  * `gitolite_user_home`: home directory for `gitolite_user` (default: `/home/{{ gitolite_user }}`)
  * `gitolite_admin_key`: gitolite administrator's public key (default: `~/.ssh/id_rsa.pub`)
  * `gitolite_admin`: gitolite administrator's name (default: `admin`)

## Dependencies

None.

## Usage

```
- hosts: all
  roles:
    - sjinks.gitolite
```

## License

MIT, see LICENSE.
