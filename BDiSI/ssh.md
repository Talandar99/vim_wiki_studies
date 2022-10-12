# using SSH via terminal

### wiki pages
- https://wiki.archlinux.org/title/OpenSSH
- https://wiki.archlinux.org/title/SCP_and_SFTP

### why?
- Windows10,Windows11 and all linux distros have ssh command built in. 
- It's easier to just open terminal and type than download GUI ssh client

### how to connect 
`` ssh -p port user@server-address ``

### how to send a file
`` scp remote_user@remote_host:/path/to/remote/file /path/to/local/file ``

### how to download file via ssh
`` scp /path/to/local/file remote_user@remote_host:/path/to/remote/file ``
