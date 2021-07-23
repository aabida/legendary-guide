# Create SSH keys

```bash
ssh-keygen -t rsa -b 4096 -f ~/.ssh/meaningful-name.key -C "My name and server DNS"
```

# Copy the key to a server

```bash
ssh-copy-id -i ~/.ssh/meaningful-name.key user@host
```

# Disable password based authentication for SSH access to server

1. Change the **PasswordAuthentication yes** to **no** in the file */etc/ssh/sshd_config*
2. ``sudo service ssh reload``
