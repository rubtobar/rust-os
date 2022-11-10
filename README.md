# From the tutorial from
https://os.phil-opp.com/minimal-rust-kernel/

# Load the OS into QEMU
qemu-system-x86_64 -drive format=raw,file=target/x86_64-rust-os/debug/bootimage-rust-os.bin