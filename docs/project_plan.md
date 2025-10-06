## Roadmap
### Phase 1:
1. Write bootloader
2. Create C kernal



## Things to learn
### phase 1 - overview:
1. Basic x86 assembly syntax (mov, jmp, int).
2. How linking and addresses work (objdump -d build/kernel.o to disassemble).
3. How make automates builds.

| Topic                                                      | Why It Matters                                                            | Working Source / Reading                                                                                                                                                                                                                                                                                                 |
| ---------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Binary & Hexadecimal**                                   | You’ll constantly deal with raw bytes, addresses, and offsets.            | SparkFun’s “Number Systems” tutorial — *Binary, Decimal, Hexadecimal* <br> ([https://learn.sparkfun.com/tutorials/number-systems/all](https://learn.sparkfun.com/tutorials/number-systems/all))                                                                                                                          |
| **CPU architecture (x86 basics, registers, instructions)** | You’ll write assembly (`mov`, `jmp`, `int`) and understand how CPU works. | OSDev Wiki: *x86 Assembly* (Assembly overview) — [https://wiki.osdev.org/Assembly](https://wiki.osdev.org/Assembly) ([wiki.osdev.org][1])                                                                                                                                                                                |
| **Boot process (BIOS, bootloader, real mode)**             | Understand how power-on leads to running your boot sector.                | OSDev Wiki: *Boot Sequence* — [https://wiki.osdev.org/Boot_Sequence](https://wiki.osdev.org/Boot_Sequence) ([wiki.osdev.org][2]) <br> OSDev Wiki: *System Initialization (x86)* — [https://wiki.osdev.org/System_Initialization_%28x86%29](https://wiki.osdev.org/System_Initialization_%28x86%29) ([wiki.osdev.org][3]) |
| **Memory addressing & real mode**                          | To know why segments like `0x7C00` / `0xB8000` are used in real mode.     | OSDev Wiki: *Real Mode* — [https://wiki.osdev.org/Real_Mode](https://wiki.osdev.org/Real_Mode) ([wiki.osdev.org][4])                                                                                                                                                                                                     |
| **VGA text buffer / screen output without OS**             | To print characters without any OS.                                       | OSDev Wiki: *VGA Text Mode* — [https://wiki.osdev.org/VGA_Text_Mode](https://wiki.osdev.org/VGA_Text_Mode)                                                                                                                                                                                                               |
| **Assembly syntax & registers**                            | You need to write small assembly stubs (bootloader).                      | nasm documentation; OSDev Wiki *Assembly* page above                                                                                                                                                                                                                                                                     |
| **Basic C syntax and compilation**                         | Kernel in C will let you shift complexity from assembly to C.             | Learn C via “Learn C in Y Minutes” (or any beginner C tutorial)                                                                                                                                                                                                                                                          |
| **Linking & binary formats**                               | To combine `.o` files into raw binary that boots.                         | Tutorials on linking bare-metal (search “bare metal linking tutorial”) <br> Example: the *Bare Bones* series in OSDev tutorials (on OSDev’s Tutorials page) — [https://wiki.osdev.org/Tutorials](https://wiki.osdev.org/Tutorials) ([wiki.osdev.org][5])                                                                 |
| **Using QEMU (virtual machine emulation)**                 | To test your OS without hardware, ease debugging.                         | OSDev Wiki: *QEMU* (via Tutorials page) — see *Getting Started* on OSDev: [https://wiki.osdev.org/Getting_Started](https://wiki.osdev.org/Getting_Started) ([wiki.osdev.org][6])                                                                                                                                         |

[1]: https://wiki.osdev.org/Assembly?utm_source=chatgpt.com "Assembly - OSDev Wiki"
[2]: https://wiki.osdev.org/Boot_Sequence?utm_source=chatgpt.com "Boot Sequence - OSDev Wiki"
[3]: https://wiki.osdev.org/System_Initialization_%28x86%29?utm_source=chatgpt.com "System Initialization (x86) - OSDev Wiki"
[4]: https://wiki.osdev.org/Real_Mode?utm_source=chatgpt.com "Real Mode - OSDev Wiki"
[5]: https://wiki.osdev.org/Tutorials?utm_source=chatgpt.com "Tutorials - OSDev Wiki"
[6]: https://wiki.osdev.org/Getting_Started?utm_source=chatgpt.com "Getting Started - OSDev Wiki"
