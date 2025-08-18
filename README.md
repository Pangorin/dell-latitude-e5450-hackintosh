# Hackintosh guide for Dell Latitude E5450, read this before doing anything!
So, this is the guide to hackintosh this deadass dumb laptop. This thing is like a snail, every mouse click will spikes up the CPU usage. Just kidding, this laptop is still usable for light coding, or watching cat videos on YouTube...

## Things you have to keep in mind
- Don't expect too much, like I said before, this laptop is quite old. Yes it's still usable, but the performance sometimes will annoy you, most likely caused by the iGPU being too weak for newer macOS.
- Since this laptop doesn't have NVMe slot, only 1 SATA SSD/HDD slot, if you're planning to install macOS above 10.15, the system responsive is quite slow. I think it will be better if you use some good SSDs like Samsung or Western Digital top-tier SSDs.
- Some base model of this laptop only have 4GB of RAM, and trust me, you don't want to use that amount of RAM on any macOS version newer than High Sierra. This laptop has 2 RAM slots, so 2 sticks of 8GB would be the best option for you.

## Specification
- Model: Latitude E5450
- CPU: i5-5300U
- RAM: 8GB
- GPU: Intel HD Graphics HD5500
- Ethernet: Intel I218-LM
- Wireless: Intel AX210, stock wireless card won't work with any macOS version, and you should pick native supported BCM wireless cards though, less problem.

## Getting started
- I will keep this guide as simple as possible, so yes, I won't rewrite the legendary OpenCore Installation Guide, do it yourself.
- You have to do the IRQ patch, *don't ask me why I know*, and my suggestion is, use the SSDTTime tool to generate ACPIs based on your system for stability. Reason for the IRQ patch is the audio problem and I have issue with internal controller(?), if I don't use this patch then some internal USB parts like webcam and Bluetooth won't work, and AppleALC can't utilize the audio controller.

## Summary
- Hackintosh this laptop is kinda fun, and I think it's quite easy to be honest.
- And as I said before, performance is the thing you really have to keep in mind. I don't use this laptop for heavy tasks, just some light coding and basic stuff like writing a document. Also using this machine with external monitor is quite limited, it worked quite well with my Dell U2419H, which is a Full HD monitor. 2K or 4K monitors are stressful for this machine, so avoid it if you can.
- If you want to use me pre-built EFI, make sure to replace the SMBIOS section, *I will probably update the config.plist to remove my current SMBIOS, because if someone use the same SMBIOS and lock this machine down then I will lose all my work stuff and have to mess up with my iCloud account*.

## Result
![Screenshot](https://github.com/Pangorin/dell-latitude-e5450-hackintosh/blob/main/images/Screenshot.png)
