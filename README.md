# RabbitMQ Broker Configuration

![img](docs/img/Incuvers-black.png)

Modified: 2021-11



## Ansible Vault
Ansible is used to manage access to the the rabbitmq broker connection credentials. These secrets are encrypted with AES using ansible vault and are version controlled. Contact <a href="mailto:christian@incuvers.com?">christian@incuvers.com</a> for the vault key file.

Install ansible:
```bash
python3 -m pip install --user ansible
```

Add the `vault.key` file to the `secrets` directory

Encrypting/Decrypting files is easy:
```bash
ansible-vault encrypt /path/to/file
ansible-vault decrypt /path/to/file
```
>Remember to always encrypt the sensitive keys before source controlling!