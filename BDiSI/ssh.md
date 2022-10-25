# Using SSH via terminal

### wiki pages
- https://wiki.archlinux.org/title/OpenSSH
- https://wiki.archlinux.org/title/SCP_and_SFTP

### why?
- Windows10,Windows11 and all linux distros have ssh command built in. 
- It's easier to just open terminal and type than download GUI ssh client

### how to connect 
- default port
`` ssh user@server_address ``
- custom port
`` ssh -p port user@server_address ``

## SCP

### how to send a file
`` scp remote_user@remote_host:/path/to/remote/file /path/to/local/file ``

### how to download file via ssh
`` scp /path/to/local/file remote_user@remote_host:/path/to/remote/file ``


## How to login with SSH password
- kenerate key ``ssh-keygen -b 521 -t ecdsa``
- we can specify ssh password, or not. If ssh is not password protected we will log in automaticly
- cd into .ssh 
- copy key to remote server `` ssh-copy-id -i id_ecdsa login@address ``
- now we can login using ``ssh 'login@address'``


## Tunneling
- we can create tunnel to maintain connection with server using L flag:
- L local_socket:remote_socket
  - example `` ssh local_socket:remote_socket login@address``
- L local_socket:host:hostport
  - example `` ssh local_socket:host:hostport login@address``


