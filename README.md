# Ubuntu-23.04-change-SSH-port
A simple solution  

Change default port by editing this file
```
sudo nano /lib/systemd/system/ssh.socket
```
Uncomment the line 'Port=22' and enter your port
```
sudo nano /etc/ssh/sshd_config
```
Then reload the daemon
```
sudo systemctl daemon-reload  
```
And restart **ssh** (it could be **sshd**)
```
sudo systemctl restart ssh
```
