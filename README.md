----------
LINUX
----------


**Show date with format**

date +"%Y%m%d %k:%M:%S"

**SSH section**

Generate ssh key pair
ssh-keygen -t rsa
ssh-copy-id -i ~/.ssh/mykey user@host

ssh -o StrictHostKeyChecking=no -i specified_directory/id_rsa user@host

**Comparison**

Numeric comparision is done using key words -eq, -ne, etc.
String comparision is done using == and !=.
[ -z ${variable} ] sends true if variable is empty
