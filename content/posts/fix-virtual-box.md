+++
title = "Fix: \"Initramfs unpacking failed\" while trying to install Ubuntu Server in Virtual Box"
date = "2021-03-13"
lastmod = "2021-03-13"
tags = [ "Virtual Box", "Linux", "Ubuntu server" ]
categories = [
    "Linux"
]
description= "Fixing unexpected virtual box error"
+++

Just posting a fix that took me hours of googling. While trying to install Ubuntu Server 20.04 on Virtual Box 6.1, and after mounting the Ubuntu Server ISO then starting the VM, I encountered this error:

{{< figure src="/images/error-screenshot.png" title="Screenshot of the error at startup" >}}

Turns out I reduced the RAM of the VM to be **512MB**, adjusting the RAM to **768MB** fixed it!

Thanks to @mrtumnus for posting his answer at serverfault:
https://serverfault.com/questions/1033384/qemu-ubuntu-server-20-04-initramfs-write-error

Hope I saved you some googling time!