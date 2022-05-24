---
title: 'Fedora Gets Stuck after Nvidia Driver and CUDA Installed'
date: 2022-05-24
permalink: /posts/2022/05/fedora-optimus-stuck/
tags:
  - fedora
  - Nvidia Optimus
  - Driver and CUDA
  - If Not True Then False
  - Stuck
---

After installing Nvidia Driver and CUDA on
a Nvidia Optimus laptop (following instructions on if-not-true-then-false),
Fedora (34+) often gets stuck after several minutes poweron.

I can not say what is wrong, but the following steps save my life:

When starting, press F10
- Modify the BIOS: turn off the CPU virtual tech (This is for problem of getting stuck)
- Modify the BIOS: Nvidia Optimus choose Discrete (This is for problem of not showing login dialogue)

And then setting Nvida GPU as PrimaryGPU:
Following the [Step #8 of Fedora DOCS](https://docs.fedoraproject.org/en-US/quick-docs/how-to-set-nvidia-as-primary-gpu-on-optimus-based-laptops/)
- Copy the nvidia config file: `sudo cp -p /usr/share/X11/xorg.conf.d/nvidia-<somethingelse>.conf /etc/X11/xorg.conf.d/`
- Open the target file: `sudo nvim /etc/X11/xorg.conf.d/nvidia-<somethingelse>.conf`
- Add the following contentto the `OutputClass` section: `Option "PrimaryGPU" "yes"`
- Then reboot
- Verify the conf: `glxinfo | egrep "OpenGL"`
