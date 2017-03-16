# fglrx_fedora-guide
How to install  AMD fglrx proprietary video driver on Fedora 25

Short version:

1. Downgrade xorg-x11-server-common xorg-x11-server-Xorg to Fedora21 versions
https://bluehatrecord.wordpress.com/2015/06/04/procedure-prototype-installing-catalyst-15-5-on-fedora-22/

2. Download devel tools:
sudo dnf install gcc kernel-headers kernel-devel

3. Download AMD fglrx proprietary video driver:
http://support.amd.com/en-us/download/desktop?os=Linux+x86_64

4. Download patcher:
https://github.com/imageguy/fglrx-for-Fedora

5.Unzip patcher files in fglrx-15.302 directory.

6.Login as root and run do_install script:
su
./do_install

7. Select the second option: "Install driver 15.302 on X.Org 6.9 or later 64-bit"

8. Install

9.After install run (as root):
aticonfig --initial

10.Reboot
