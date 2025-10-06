## Roadmap
### Phase 1:
1. Write bootloader
2. Create C kernal



## Things to learn
### phase 1 - overview:
1. Basic x86 assembly syntax (mov, jmp, int).
2. How linking and addresses work (objdump -d build/kernel.o to disassemble).
3. How make automates builds.

| Topic                                            | Why It Matters                                                                                | Resources (good for beginners)                                                                                                                                                    |
| ------------------------------------------------ | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Binary & Hexadecimal**                         | You’ll constantly deal with raw bytes, addresses, and offsets.                                | 🔹 Crash Course Computer Science Ep 6: *The Binary System* (YouTube) <br> 🔹 [“Binary, Decimal, Hexadecimal”](https://learn.sparkfun.com/tutorials/number-systems/all) — SparkFun |
| **CPU architecture (x86 basics)**                | You need to know what registers (`ax`, `bx`, etc.) and instructions (`mov`, `jmp`, `int`) do. | 🔹 [x86 Assembly Crash Course – Kalle Hallden / 3Blue1Brown style](https://youtu.be/75gBFiFtAb8) <br> 🔹 [OSDev Wiki: x86 Assembly Primer](https://wiki.osdev.org/X86_Assembly)   |
| **Boot process (BIOS, bootloader, real mode)**   | The first code the CPU runs and how it loads your boot sector.                                | 🔹 [OSDev Wiki: Boot Sequence](https://wiki.osdev.org/Boot_Sequence) <br> 🔹 [Ben Eater – 16-bit BIOS bootloader video](https://www.youtube.com/watch?v=HCf1XzoxG3U)              |
| **Memory addressing (segmentation & real mode)** | Why 0x7C00 and 0xB8000 matter; how BIOS maps RAM.                                             | 🔹 [Real Mode Memory Map (OSDev)](https://wiki.osdev.org/Memory_Map_%28x86%29)                                                                                                    |
| **VGA text buffer**                              | How to print without an OS.                                                                   | 🔹 [VGA Text Mode – OSDev Wiki](https://wiki.osdev.org/VGA_Text_Mode)                                                                                                             |
| **Assembly syntax & registers**                  | You’ll write boot.asm manually.                                                               | 🔹 [nasm official manual](https://www.nasm.us/xdoc/2.16.01/html/nasmdoc1.html) (skim)                                                                                             |
| **Basic C syntax and compilation**               | Needed for kernel.c.                                                                          | 🔹 [Learn C in Y Minutes](https://learnxinyminutes.com/docs/c/) <br> 🔹 [K&R “The C Programming Language” book, chapters 1-5] (classic, short)                                    |
| **Linking & binary formats**                     | You’ll link `.o` into raw binaries and understand `ld` scripts.                               | 🔹 [“Bare metal C: linking & sections”](https://interrupt.memfault.com/blog/arm-linker-script) (ARM-focused but conceptually right)                                               |
| **Using QEMU**                                   | Lets you test without hardware.                                                               | 🔹 [QEMU for Beginners – OSDev Wiki](https://wiki.osdev.org/QEMU)                                                                                                                 |


