# Aleo Workshop 1 Task 

## Build Guide

To compile this Aleo program, run:
```bash
snarkvm build
```

To execute this Aleo program, run:
```bash
snarkvm run hello
```

Changed the unsigned integer byte from u32 to u16
``` bash
program hello.aleo {
    transition main(public a: u16, b: u16) -> u16 {
        let c: u16 = a + b;
        return c;
    }
}
```
Run
```bash
leo run main 5u64 5u64
```
