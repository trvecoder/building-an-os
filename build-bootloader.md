# What did we do?
- installed nasm (assembler) and qemu(test os) 

bios/bootloader/os
- BIOS:	Like the ignition in a car — it starts the system
- Bootloader (512 bytes):	Like a car key — it decides what to start
- OS:	Like the engine that actually drives everything

| Real Computer Boot             |  QEMU       |
| ------------------------------ | --------------------------- |
| Turn on PC                     | Run `qemu-system-x86_64`    |
| BIOS loads 512 bytes from disk | QEMU reads `bootloader.bin` |
| BIOS runs bootloader           | QEMU jumps to `0x7C00`      |
| Screen shows boot output       | QEMU window shows text      |
