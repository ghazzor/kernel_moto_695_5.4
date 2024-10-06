### Kernel Source For `SM6375/SD695`

**Based on [`android_kernel_motorola_sm6375`](https://github.com/Motorola-SM6375-Devs/android_kernel_motorola_sm6375)** 

#### **Features**

- Compiled with `Neutron Clang 18`
- LLVM Polly
- Inline Optmizations
- Some Debugging Nuked
- Wireguard

#### **Build Instructions**

```shell
# Dependencies for ubuntu
$ sudo apt install bash git make flex bison build-essential libssl-dev curl bc pkg-config m4 libtool automake autoconf zstd libarchive-tools wget

# Clean build for g84, ksu
$ KSU=1 ./build.sh -c

# Dirty build for g34 , no ksu
$ DEVICE=g34 KSU=0 ./build.sh -d
```
Toolchain is synced automatically

Flashable zip is localted in Anykernel3/O_KERNEL*.zip

### **Note**
1. G34 builds do no boot (will fix it later).

### **Credits** *(kanged everything from these guys)*

- **[`@AnandSuresh02`](https://github.com/AnandSuresh02)** (base tree)
