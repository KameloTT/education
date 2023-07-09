# SSH - Remote access

ssh is a tool which allows to connect to remote laptop/server.

Usually all laptops/servers on linux/MacOs have such tool.

##  Access with login/password

Below is syntax of using

```
ssh <user>@<server_name or ip>
```

Example:

if we want to connect to server with ip **10.211.55.9** with user **user1**

```
ssh user1@10.211.55.9
```

Terminal asks password for user1 to allow access to 10.211.55.9

Once you enter correct password for user1 you will be able to login to 10.211.55.9 server.

## Passwordless access

In automation world, scripts sometimes are required to connect to remote servers for running some commands and it is unacceptable to enter password manually each time when your script tries to connect to remote server.

For such scenario where we need to get access to remote server without password we need to create special ssh key which we can use as atrust proof for remote server.

Step 1. Create new ssh key.

We use toolwith name ssh-keygen which generates two keys.

- Public key - we copy such key to remote server
- Private key - out personal key which we will use to remote connect to server with preinstalled our public key

???+ note

     Public key is always assosiate only with one single private key. Pair public/private keys  is uniq. We can create many public/private keys but specific public key always belong to their private key which is generated at the same time.


```
ssh-keygen
```

Press Enter on all questions. it will create private/public key pair in default place

<img src="../img/ssh-1.png" />

Step 2. Locate your keys

```
ls -l ~/.ssh/
```

- id_rsa - is private ssh key
- id_rsa.pub - is public ssh key

Step 3. Use ssh keys for passwordless remote connection

For using such key we need to add our public ssh key to remote host

```
ssh-copy-id -i ~/.ssh/id_rsa.pub user1@10.211.55.9
```
Enter password

<img src="../img/ssh-2.png" />

Login to remote host with using our own ssh private key

ssh -i ~/.ssh/id_rsa user1@10.211.55.9


## Execute remote command via ssh on remote host

ssh tool allows us to run command on remote host as well as just login to one

```
Syntax: ssh -i <private_key> <user>@<host> <command>
```

Example:

```
ssh -i ~/.ssh/id_rsa user1@10.211.55.9 date
```

Such command run command **date** which shows time and date on remote server.

<img src="../img/ssh-3.png" />
