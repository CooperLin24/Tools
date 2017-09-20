configuration for sharing kerboard and mouse between Ubuntu and Windows:
# download Synergy
# Install Synergy in Ubuntu
    $ sudo dpkg -i synergy-v1.7.3-stable-efd0108-Linux-x86_64.deb
Config Ubuntu as a server:
    $ vim /home/${username}/synergy.conf

section: screens
DESKTOP-9T2Q40K:
shunlqing-B85-D3V:
end

section:links
shunlqing-B85-D3V:
left = DESKTOP-9T2Q40K
DESKTOP-9T2Q40K:
right = shunlqing-B85-D3V
end

# Start synergy in Ubuntu:
    $ synergys -f --config /home/${username}/synergy.conf
    (Can chonse write the commad to a shell and cp to /usr/sbin)
# Install Synergy in Windows
    Config windows as a client with server's IP then start.


