### Kernel Source For `SM6375/SD695`

**Fork of [`android_kernel_motorola_sm6375`](https://github.com/Motorola-SM6375-Devs/android_kernel_motorola_sm6375)**

#### **Features**

- Compiled with `Neutron Clang 18`
- LLVM Polly
- Inline Optmizations
- Debugging Nuked
- Wireguard
- KSU Next
- Minor optimizations
- Full kernel inline (i.e. no modules excet nfc)

#### **Build Instructions**

```shell
# Dependencies for ubuntu
$ sudo apt install bash git make flex bison build-essential libssl-dev curl bc pkg-config m4 libtool automake autoconf zstd libarchive-tools wget

# Clean build for g84, ksu
$ KSU=1 ./build.sh -c

# Dirty build for g84 with goodix display, no ksu
$ DEVICE=g84_gdx KSU=0 ./build.sh -d
```
Toolchain is synced automatically

Flashable zip is localted in Anykernel3/O_KERNEL*.zip

### **Note**
1. G34 builds do no boot (won't fix) (pull reqs are welcome).
2. NFC is broken if not compiled as a module, so that is the only module in the kernel.

### **Credits** *(kanged everything from these guys)*

- **[`@AnandSuresh02`](https://github.com/AnandSuresh02)** (base tree)
