# VcXsrv-Linux-Windows-Bridge

## Step 1: SSH

```
#pacman -S openssh
#ufw allow 22 && ufw limit ssh
#systemctl enable sshd
#systemctl start sshd
```

Regular ssh into your user. `ssh user@ip`
[Download VcXSrv](https://vcxsrv.com/)

## Step 2: SSH X
```
ssh -X user@ip
export DISPLAY=WINDOWS_IP:0
export XAUTHORITY=$HOME/.Xauthority
```

You can then launch any app like you would normally. 

![X11DIRECTACCESS](https://github.com/h8d13/LSK---Linux-Starter-Kit/blob/main/media/capcap.PNG)
