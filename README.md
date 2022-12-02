# From the tutorial from
https://os.phil-opp.com/minimal-rust-kernel/

# The builder assumes that you have installed build-essentials
```bash
sudo apt install build-essential
```

# Install bootimage to binary to the system Load
```bash
cargo install bootimage
```

# For running bootimage and building the bootloader, you need to have the llvm-tools-preview rustup component installed
```bash
rustup component add llvm-tools-preview
```

# After installing bootimage and adding the llvm-tools-preview component, we can create a bootable disk image by executing
```bash
cargo bootimage
```

# Load the OS into QEMU
```bash
qemu-system-x86_64 -drive format=raw,file=target/x86_64-rust-os/debug/bootimage-rust-os.bin
```

# TODO: Newlines
