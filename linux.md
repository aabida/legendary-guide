
----------
LINUX
----------


**Show date with format**

date +"%Y%m%d %k:%M:%S"

**Comparison**

Numeric comparision is done using key words -eq, -ne, etc.  
String comparision is done using == and !=.  
[ -z ${variable} ] sends true if variable is empty

**Copy files from and to a remote server**
```bash
scp your_username@remotehost.edu:foobar.txt /some/local/directory  
scp foobar.txt your_username@remotehost.edu:/some/remote/directory  
```

**SSH key generation**

```bash
ssh-keygen -t rsa  
ssh-copy-id -i ~/.ssh/mykey user@host  
ssh -o StrictHostKeyChecking=no -i specified_directory/id_rsa user@host
```

**Communicate with a resmote server using ssh**

To execute a given script file in a remote server using ssh command :  
```bash
ssh -i path/to/private/key user@server "cat | bash /dev/stdin" < script-file.sh  
```
To pass parameters to the script, add it after /dev/stdin as here:  
```bash
ssh -i path/to/private/key user@server "cat | bash /dev/stdin param1 param2" < script-file.sh  
```
Note : the default private key that will be used is in ```$HOME/.ssh/id_rsa```

## Add a program to Ubuntu launcher
You will be able to add a shortcut to an application

All the shortcuts are in the directory *~/.local/share/applications*.
Create a new file in the directory and add the following content :
```bash
[Desktop Entry]
Type = Application
Name = name-of-application
Comment = your-desired-comment
Exec = command to execute (ex. 'eclipse')
Icon = path-to-icon
```
## Upgrade applications and diffrent commands
```bash
sudo apt full-upgrade
```
Reference : [lecoindunet.com](https://www.lecoindunet.com/difference-apt-update-upgrade-full-upgrade)
