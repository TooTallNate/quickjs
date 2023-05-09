The main documentation is in doc/quickjs.pdf or doc/quickjs.html.

Compile for DevkitPro A64:

export PATH="/opt/devkitpro/devkitA64/bin:$PATH"
make ARMCPU=cortex-a57 ARMLINUX=yes CROSS_PREFIX=aarch64-none-elf- CFLAGS="-march=armv8-a+crc+crypto -mtune=cortex-a57 -fPIE -I/opt/devkitpro/devkitA64/aarch64-none-elf/include -DCONFIG_BIGNUM" LDFLAGS="-L/opt/devkitpro/devkitA64/aarch64-none-elf/lib" libquickjs.a
