# Linux-Windows-Bridges

## Step 1: SSH
```
#pacman -S openssh
#ufw allow 22 && ufw limit ssh
#systemctl enable sshd
#systemctl start sshd
```

Regular ssh into your user. `ssh user@ip` Check it works all good. 

[Download VcXSrv](https://vcxsrv.com/)

## Step 2: SSH X
```
ssh -X user@ip
export DISPLAY=WINDOWS_IP:0
export XAUTHORITY=$HOME/.Xauthority
```

You can then launch any app like you would normally. 

![X11DIRECTACCESS](https://github.com/h8d13/LSK---Linux-Starter-Kit/blob/main/media/capcap.PNG)

Alternatively: RustDesk works good and has .exe files for windows

I also found this gist which seems to be able to use the standard RDP from Windows: https://gist.github.com/valorad/7fd3e4a7fb4481f1eb77ded42a72537d
But it's too much work for what it is. 
