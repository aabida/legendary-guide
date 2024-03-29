# Create SSH keys

```bash
ssh-keygen -t rsa -b 4096 -f ~/.ssh/meaningful-name.key -C "My name and server DNS"
```

# Copy the key to a server

```bash
ssh-copy-id -i ~/.ssh/meaningful-name.key user@host
```
This command will add the public key to **~/.ssh/authorized_keys** file

# Connect to the server using the generated key

```bash
ssh -i ~/.ssh/meaningful-name.key user@host
```

# Disable password based authentication for SSH access to server

1. Change the **PasswordAuthentication yes** to **no** in the file */etc/ssh/sshd_config*
2. ``sudo service ssh reload``

# Reference
- https://www.ssh.com/academy/ssh/authorized-keys-file
- https://www.ssh.com/academy/ssh/copy-id
- https://www.e2enetworks.com/help/knowledge-base/how-to-enable-disable-password-based-authentication-for-ssh-access-to-server/
- https://qastack.fr/ubuntu/1991/disable-password-access-through-ssh
