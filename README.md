# shuttlexpress_linuxcnc
HAL file for using shuttlexpress as pendant in linuxcnc 2.8

Being new to linuxcnc, I wanted to test out using a pendant to controll my cnc router.
I purchased a Shuttlexpress, because I had seen reviews and though it would work "out-of-the-box".
Well, I soon found out that it did not.

In order to make it work I found that I needed to have a HAL file for it.

I didn't know what that was. And I didn't know where to put a HAL file.
Some quick searches gave me that information, but finding a HAL file that worked for shuttlexpress was not that easy.

Changes in HAL API between different linuxcnc revisions makes things even more complicated because a lot of information
out there cannot be used as-is because the information is only correct for older versions of linixcnc.
I'm using 2.8.

But after struggling for some hours I found the info I needed in this post by John Dammeyer at the end of a "Adding a ShuttleXpress" thread:
https://forum.linuxcnc.org/24-hal-components/37042-adding-a-shuttlexpress?start=30

I'm sure that I had seen it before, but it was only until I read the last post by "mudnaes" I realized that the John Dammeyers post actually contained an attachment.

I tested it out at it gaves some errors. I fixed those and it worked! If I had read the last post by "mudnaes" carefully I would have seen that he mentions those errors:
"If you dont have A-axis just comment out anything to do with joint.3. If you dont, you will get an error when starting LinuxCNC."

Anyway, I've pushed this file to github to keep it stored somewhere. But John Dammeyer deserves all credit.







