# Ansible Role: AuthKeys-Check

This role provides a shell script (to run by cron) that checks if ~/.ssh/authorized_keys file was changed. 

## Requirements

 - coreutils
 - diffutils

## Role Variables

See `defaults/main.yml` for details.

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
         - { role: classyllama.authkeyscheck, tags: authkeyscheck, when: use_classyllama_authkeyscheck | default(false) }

## License

This work is licensed under the MIT license. See LICENSE file for details.
