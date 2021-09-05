# Check a port is taken by which program on Linux
    netstat -tunlp | grep [port]

Ref: [https://www.pixelstech.net/article/1534063164-How-to-check-a-port-is-taken-by-which-program-on-Linux]

# Stop program running at startup in Linux
https://unix.stackexchange.com/questions/13/stop-program-running-at-startup-in-linux

## To list all the startup services

    systemctl
## To stop a service from running on start up

    sudo systemctl disable servicename
### For instance if we need to stop running ssh server at startup

    sudo systemctl disable sshd.service
## We can enable this again using

    sudo systemctl enable sshd.service

Almost every linux distributions use systemd for bootstrapping startup services. So above commands work for most of the distros.
