# G15-5515-Ryzentosh 

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


| Component | Status | Compatible? |
|-----------|--------|-------------|
|CPU: AMD R7 5800H  | CPU supported,detected as intel core i5|  ✅|
|iGPU: AMD Vega 8| GPU supported, Metal2 API capable|  ✅|
|WiFi : Killer AX600| supported,detected as intel AX600 |✅|
|Bluetooth: Killer AX600| supported,detected as intel AX600| ✅|
|Speakers|supported|✅|
|Built in Webcam| supported|✅|
|FaceTime, iMessage, Apple Services| supported|✅|
|Screen|supported, both 120hz and 60hz modes available with pro-motion|✅|
|Keyboard|supported, with different backlight levels|✅|
|USB Ports| supported, all running at full speeds| ✅|
|SODIMM slots & Memory| supported, all 64 gigs detected|✅|
|Trackpad|supported, detected as ps2 mouse|🚧|
|Storage| partially supported, Crucial drive acting as main drive, SK Hynix drive disabled in ACPI patches to prevent KP | 🚧|
|dGPU: Nvidia RTX 3050Ti| GPU not supported even by web drivers |❌|
 

<h2>Supported (and verified) macOS versions:</h2>

- macOS Monterey
- macOS Ventura

<h2>Some Screenshots:</h2>

No Stage Manager: 

![Screenshot 2023-08-08 at 6 08 04 PM](https://github.com/chcheetah/G15-5515-Ryzentosh/assets/79366050/6e2312c3-5168-40ab-a111-0971f06cfacd)

With Stage Manager:
![Screenshot 2023-08-08 at 6 41 46 PM](https://github.com/chcheetah/G15-5515-Ryzentosh/assets/79366050/e3b66234-f0ec-4790-a2f1-2e32f67e5143)



<h2> Disclaimer: </h2>

Do note that this project is intended solely for personal educational use and not for commercial use.


|<h2> Credits</h2>|
|----|
|Apple for macOS
|OpenCore for the EFI|
|NootedRed for the AMD iGPU kext|
|the Hackintosh Community for all the kexts|



