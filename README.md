LightDM Webkit Arch Theme
===========================

This is a LightDM webkit greeter theme for Archlinux. Based on [LightDM-Webkit-MacOSX-Theme](http://github.com/Wattos/LightDM-Webkit-MacOSX-Theme)


[ Fork changes ]
I just have made some changes in login input box style and changed the avatar color to white. 
Also made some changes in sytle of WM selector. But it is not working in my Arch. I think that is a bug with LightDM
webkit of AUR.

I hope that you enjoy it :D
[ That's all folks! ]

Installation Instructions
-------------------------
You will need lightdm as your login manager and the lightdm-webkit-greeter from AUR. You need to make the webkit greeter the default greeter. This is done by editing the lightdm configuration under:

<pre>
/etc/lightdm/lightdm.conf
</pre>

and changing the greeter-session value to lightdm-webkit-greeter. lightdm.conf should have:

<pre>
[SeatDefaults]
greeter-session=lightdm-webkit-greeter
allow-guest=false
</pre>

The second step is to install the actual theme. This is done by copying the files of this repository into the following location:

<pre>
/usr/share/lightdm-webkit/themes/arch
</pre>

Finally, change the /etc/lightdm/lightdm-webkit-greeter.conf file to contain the following line:

<pre>
webkit-theme=arch
</pre>

Now you can reboot and enjoy the new theme.
