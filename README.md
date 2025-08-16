# Hackintosh guide for Dell Latitude E5450
So, this is the guide to hackintosh this deadass dumb laptop. This thing is like a snail, every mouse click will spikes up the CPU usage. Just kidding, this laptop is still usable for light coding, or watching cat videos YouTube...

## Things you have to keep in mind
- Don't expect too much, like I said before, this laptop is quite old. Yes it's still usable, but the performance sometimes will annoy you.
- Since this laptop doesn't have NVMe slot, only 1 SATA SSD/HDD slot, if you're planning to install macOS above 10.15, the system responsive is quite slow.
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
- Hackintosh this laptop is kinda fun
