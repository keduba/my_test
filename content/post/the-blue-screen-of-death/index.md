---
title: the Blue Screen of Death
subtitle: How to save your files easily when you find yourself at this crossroad
date: 2022-03-16T06:55:11.346Z
draft: false
featured: false
tags:
  - Tutorial
categories: []
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
## Tutorial

### Outline

* Backing up the files
* If all fails, try a Linux USB
* Run a try (not install) of the Linux.
* Mount the disk  and look at your files and directories.
* Take note of the filesystem architecture and layout
* Write it on paper to help you when you are going to replace them.
* Compress files and directories
* Save online or copy to external drive
* Format disk using GParted or disk manager
* Reinstall Windows or Install Linux
* Restart the computer
* Replace the files.

### Backing up your files

This is not a solution to the blue screen of death (BSOD). No it is a measure of precaution that you should apply so as not to lose time if and when BSOD hits. There are many ways to backup your files. I shall not dwell on the details now but I shall write a post about it and link to it here.

However two simple ways are to:

* Use an external hard disk or a USB stick.
* Back up to an online storage system or server.
  This will help you when the evil day arrives though I hope it never does.

### Try a Linux USB

Having a USB from which you can run Linux will save your life many times over. The reason for saying this is that even if you have a Windows Installer, there are times when the boot loader of your existing Windows is so far gone that it won't be able to run another Windows installer.

On the other hand, you can run a Linux OS from a flash drive without needing to install it and still be able to do most things *if not everything* with your computer. I'm actually tempted to say, everything instead of most things.

### Getting the Linux on a USB

If you are at this point, you'll need to create your installable device. There are several tools that can do the job depending on your circumstances.

A. You are surrounded by Windows computers:

* If this is you, then my go to tool is [rufus](https://rufus.ie). It's small and lightweight, and it runs fast. Download it.
* Get a Linux `.iso` image. There are so many Linux distributions **(distros)**. Since you just want something you can use to rescue your files, then there's no need to go fancy. anyu of the [Ubuntu](https://www.ubuntu.com) flavours will serve. You can get either Ubuntu, [Kubuntu](https://www.kubuntu.org), [Xubuntu](https://www.xubuntu.org) assuming you don't know where to start from. If you already have a preference, you can go for it even if it's not among my suggestions.

B. You have a Linux:

* There are native disk creators. Search for this term on you Linux PC and it should briing up the application for you. If you don't find it, you can try [Ventoy](https://www.ventoy.net). The good thing about Ventoy is that it allows you to write multiple OS `.iso`'s without blinking. Then you can pick and choose. After the initial setup, having an OS is as simple as copying the .iso file to the flash drive.
* After it's downloaded, run `rufus`, selecting the `.iso`, choosing **GPT** for the partition type. Most of the default settings work just fine. Hit `START`, accept the warning and come back around 3 - 6 minutes.
* I have to say that this process is going to be run on a different computer whether a spare one, a friend's or at the library because we are assuming that your computer is currently comatose and on life support.

### Run your new disk installer

Your last step should have been successful. Now is the moment of truth. Are you ready? Bist du vertig?

* Plug in the sick laptop. It should be on life support.
* Plug in the USB stick.
* Note your `Esc`, `Enter` or `Fn` keys. One of them will help you get into the boot options.
* Power on the computer.
* Hit the key you need to go to the setup. HPs, think `ESC`; Lenovo, think `Enter`.
* Usually select `F9` or `F10` to go select Boot options. This varies by computer brand.
* Select *Boot from USB* or a variation of this.
* If your flash drive has only one OS installed, then it will start up right away.
* Select the first option. Allow it to load.
* It shows you the *Try* and *Install* options page.
* Select *Try from the CD*. It is going to load it up for you.

### Mount the disk

When you have successfully gone through the preceding steps, your hard disk filesystem should be available to you as a disk attached to the computer. At this point you should be access it by mounting it. If you were to double-click on it, it should be mounted automatically for you.

### Go through your filesystem.

This part is important because you might want to preserve the structure of the old system you had in Windows to enable you to reach certain files easily. Depending on how you intend to create a backup, it is advisable to write down or at least note in writing the general structure of what is there.

If all you care about is getting the files out, then you might not entirely care but to prevent stress, you should care a little.

### Preparing your backup and extraction

At this point, a good idea is to check the size of your folders and files. Large folders and files can be an encumbrance if you have a limitation of size on your backup devices such as external hard drive. If that it not the case, then there's nothing to worry about.

* You can compress the files and folders using `tar` to any archive format of your choice. This will help you preserve the structure, and you will only need to extract the files afterwards to continue your work.
* Shortcut to use `tar` to compress a file to `sample` format:

### Backup (Online or Offline)

After you have prepared your files for the backup, you can send them to the external disk if you have one, or you upload them to an online storage service. 

In the absence of a dedicated online storage service or an external hard disk, you can also use a file sharing service that keeps files for about a week or at least several days. This should give you sufficient time to sort your computer out.

* If you use the file sharing service (of which there are many safe and secure ones), be sure to write down or copy the links to the files so that you can use it to download the files when you are done.

### Installing a new OS

The new OS could be a reinstallation of the Windows OS you prefer. Otherwise, if you liked the OS you used to get your files back, you can simply hit the install button that it shows you. On the chance that you don't entirely like its appearance, you can simply shut it down.

Get an OS you like and follow the steps we highlighted earlier till you get to the Try or Install page. Then hit install, if it's a Linux version.
If it is Windows, you'll follow the Windows prompts.
It should format the disk and make the necessary partitions for you.

### Replace the files

Supposing that everything has gone well until this point, then all you need to do is put your files back. Download them from the online service you used (storage service or file sharing service) or copy them from your external hard disk.

### Restart

Literally, start all over and enjoy your *new* computer.