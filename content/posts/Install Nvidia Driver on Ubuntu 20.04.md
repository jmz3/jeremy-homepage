+++
title = "Install Nvidia Driver on Ubuntu 20.04"
subtitle = "Technical Blog"
author = "Jiaming Zhang"
date = "2023-02-01"
weight = 11
description = "A specific guide about installing nvidia drivers on machine hosting Ubuntu OS."
categories = ["technical","guide"]
tags = ["Ubuntu","Nvidia","GPU"]
menu = "main:posts"
#draft = "true"
plotly = "true"
image = "/images/blog.png"
+++


>**Environment**
<br>
<u>Hardware</u>: Lenovo y9000p 2019 - intel i7-9750H<br>
<u>OS</u>: Ubuntu 20.04 LTS Dual Boot<br>
<u>Kernel version</u>: Linux 5.13.0-39-generic<br>
<u>GPU model</u>: GTX 1660 Ti 6GB<br>

# Install Nvidia Drivers through GUI
![test img](/static/images/test.png)

choose the right tested driver version via Software & Updates - Additional Drivers; then click apply changes

wait for it to download and configure the drivers. 

After that, a window will prompt out to tell you you need to set up a key for secure boot. Type in whatever you want, just try to record/remember what you just type.

Then a restart button will appear right next to the "Revert" and "Apply changes" button. Click it. After restart, you might see a blue screen shown "perform MOK management" , then you can select "enroll MOK" and enter the key you just set for secure boot.

![在这里插入图片描述](https://img-blog.csdnimg.cn/a96a4c3daec349e39a27602aac320ff8.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBA5bCP5byg5oOz5aW95aW95a2m5Lmg,size_20,color_FFFFFF,t_70,g_se,x_16)
# Potential Bugs...

For Lenovo motherboard, you'll probably encounter a problem that you cannot type in the MOK key through Keyboard when you restart your computer. Your computer seems to stuck at the perform MOK management page and nothing can be input. And the keyboard seems to fail.

The reason is that, MOK management GUI starts even before the Input devices are initialized. The input devices are not brought up and therefore you cannot use keyboard to type in anything.

To fix that, you should first shut down the computer and boot it to jump-over the MOK step. This operation will deactivate your Nvidia Driver either, so you have to repeat the previous steps to select the right driver version and reboot your laptop.

But pay attention, this time you have to click F2 really fast to directly go into BIOS interface before the MOK management GUI shows up. If you succeed, you will find out that keyboard is now ready to use. Now you can exit the BIOS directly. If everything goes well, you'll see the MOK management GUI again but this time your keyboard is available!

![在这里插入图片描述](https://img-blog.csdnimg.cn/85b6a33de0b14cd9acf34980a38c855c.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBA5bCP5byg5oOz5aW95aW95a2m5Lmg,size_17,color_FFFFFF,t_70,g_se,x_16)
![在这里插入图片描述](https://img-blog.csdnimg.cn/3370b27d507e42d1a749d6a9bd95ef19.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBA5bCP5byg5oOz5aW95aW95a2m5Lmg,size_20,color_FFFFFF,t_70,g_se,x_16)
[https://unix.stackexchange.com/questions/608217/keyboard-does-not-work-in-mokmanager-during-key-enrollment](https://unix.stackexchange.com/questions/608217/keyboard-does-not-work-in-mokmanager-during-key-enrollment)


