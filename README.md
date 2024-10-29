# G15-5515-Ryzentosh 


Update 2.0 is out (29/10/24)!

Some bug fixes/patches applied to EFI :

1. Working trackpad gestures!!!!
2. Less microstutter throughout the system when running Ventura.
3. No usb controller bugs during the boot process.
4. Changed device type from iMac Pro to MacBook Pro.


<h2> A mandatory sea shanty 😄</h2>
<pre>
Oh, I had a dream one night so bold,
Of running systems, stories untold,
Windows, Linux, macOS so fine,
On my personal machine, a dream of mine.

Sailing 'cross the digital sea,
A tech adventure, wild and free,
But obstacles came, tried to dismay,
Yet heroes arose to pave the way.

Apple's Silicon, a mighty tide,
Swept away hopes, left me in a stride,
No AMD iGPU love to be found,
In macOS land, my dreams near drowned.

Sailing 'cross the digital sea,
A tech adventure, wild and free,
But heroes emerged, determined and bright,
@NootedRed crew, in the heart of the fight.

With skill and code, they labored long,
To create a kext, to right the wrong,
A working display, for AMD's might,
In macOS realm, they shed the light.

Sailing 'cross the digital sea,
A tech adventure, wild and free,
@NootedRed crew, with talents so vast,
They brought my dream, from shadows to cast.

Armed with the kext, I sailed ahead,
Onward I pushed, no challenge I'd dread,
A macOS laptop, complete and grand,
Most functions alive, across the land.

Sailing 'cross the digital sea,
A tech adventure, wild and free,
Though dGPU's absence brings a sigh,
My dream's alive, reaching for the sky.

So here's to dreamers and to those who strive,
To make the impossible come alive,
Through challenges faced and barriers crossed,
Tech's brave pioneers, no matter the cost.
</pre>
<b> TLDR: Silicon dreams sailed,  NootedRed's light pierced the storm,  Mac's realm, AMD's form.</b>
<h2>Current EFI scenario (listed in order of functionality)</h2>


| Component | Status (Initial) | Status (Update 2.0) |Initial Release Comments| Update 2.0 Comments |
|-----------|--------|-------------|---------------|-------------|
|CPU: AMD R7 5800H |  ✅|  ✅ | CPU supported,detected as Intel Core i5| CPU supported & detected as Ryzen CPU|
|iGPU: AMD Vega 8|  ✅ |  ✅ | GPU supported, Metal2 API capable|  GPU supported, Metal3 API capable|
|WiFi : Killer AX600|   ✅ | ✅ | supported, detected as intel AX600| supported, detected as intel AX600|
|Bluetooth: Killer AX600|   ✅ |  ✅| supported,detected as intel AX600| supported, detected as intel AX600|
|Speakers|✅|  ✅|supported|supported|
|Built in Webcam|  ✅|✅|supported|supported|
|FaceTime, iMessage, Apple Services|  ✅|✅|supported|supported|
|Screen|  ✅|  ✅| supported, with promotion| supported, with promotion |
|Keyboard|   ✅|  ✅| supported, with different backlight levels| supported, with different backlight levels|
|USB Ports|   ✅  | ✅|supported, all running at full speeds| supported, all running at full speeds|
|SODIMM slots & Memory|   ✅|  ✅|supported, all 64 gigs detected|supported, all 64 gigs detected|
|Trackpad|🚧| ✅|supported, detected as ps2 mouse|supported, with all apple trackpad gestures available|
|Stability|❌|✅| microstutters, and unable to sleep without errors. | no microstutters, able to sleep without errors|
|USB issue| 🚧| ✅| requires constant plugging & unplugging of usb devices to boot, otherwise KP | fixed now using GenericUSBXHCI.kext, no such requirement during boot |
|Storage| 🚧| 🚧| partially supported, Crucial drive acting as main drive, SK Hynix drive disabled in ACPI patches to prevent KP |partially supported, Crucial drive acting as main drive, SK Hynix drive disabled in ACPI patches to prevent KP  |
|dGPU: Nvidia RTX 3050Ti|❌|❌| GPU not supported even by web drivers, disabled. |GPU not supported even by web drivers, disabled.|
 

<h2>Supported (and verified) macOS versions:</h2>

- macOS Monterey
- macOS Ventura

<h2>Some Screenshots:</h2>

No Stage Manager: 

![Screenshot 2023-08-08 at 6 08 04 PM](https://github.com/chcheetah/G15-5515-Ryzentosh/blob/main/Images/Screenshot%202023-08-08%20at%206.08.04%20PM.png)

With Stage Manager:
![Screenshot 2023-08-08 at 6 41 46 PM](https://github.com/chcheetah/G15-5515-Ryzentosh/blob/main/Images/Screenshot%202023-08-08%20at%206.41.46%20PM.png)



<h2> Disclaimer: </h2>

Do note that this project is intended solely for personal educational use and not for commercial use.


|<h2> Credits</h2>|
|----|
|Apple for macOS|
|OpenCore for the EFI|
|NootedRed for the AMD iGPU kext|
|the Hackintosh Community for all the kexts|



