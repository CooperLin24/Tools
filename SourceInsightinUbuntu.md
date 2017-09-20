# sudo apt-get install wine
workpath : ~/.wine
# setup si.exe
$ wine si.exe
find install path in ~/.wine/drive_c/Programe File/...
# startup
vim startsi.sh with :
```
#!/bin/bash
wine "c:\Program Files (x86)\Source Insight 3\Insight3.exe" &
```
chmod a+x startsi.sh
sudo cp startsi.sh /usr/sbin/
startsi.sh
