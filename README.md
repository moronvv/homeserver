# homeserver

IaC for homeserver on Raspberry Pi

## preinstall

1. `brew install ansible`
1. `ssh-keygen -o -a 100 -t ed25519 -f ~/.ssh/homeserver -C <email>`
1. `ssh-copy-id -i ~/.ssh/homeserver <username>@<hostname>[:<port>]`
1. Create file `.vault_pass` with password for `secret.yml` vault
1. `ansible-playbook run.yml -K` on first run with password

## run

```sh
ansible-playbook run.yml
```
