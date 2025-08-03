## Minimal AC'97 VirtualBox Sound driver for TempleOS/TinkerOS

This provides sounds similar to that of a PC Speaker mainly for VirtualBox which doesn't support the PC Speaker or awesome Adlib sounds that TinkerOS supports.

Notes:
- Performance will be bad if you don't have good hardware or are not using hardware acceleration for your virtual machine.
- This is mainly for Windows people, if you're running Linux it will work, but you will get much better sound if you, compile the VMusic extension and use TinkerOS with Adlib instead!
- This is for VirtualBox only, it will not work properly in QEMU!  In QEMU use PC speaker for TempleOS `-audiodev sdl,id=snd0 -machine pc,pcspk-audiodev=snd0` or Adlib for TinkerOS instead `-audiodev sdl,id=snd0 -device adlib,audiodev=snd0` and you will get much better sound and can even change to different instruments.

## TempleOS VirtualBox setup
- Get TempleOS ISO with AC97 included (`TempleOS_AC97.ISO`) under assets from [here](https://github.com/tinkeros/TinkerOS-AC97/releases/tag/TempleOS_AC97)
- Use Windows XP 64-bit for the OS (this should default to the correct IDE drive setup and ICH AC97 sound driver), at least 2 CPU cores, at least 4 GB RAM, and set the pointing device type to PS/2 Mouse in the VM settings.
