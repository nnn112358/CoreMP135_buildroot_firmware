# CoreMP135_buildroot_firmware

buildroot (kernel 6.1)
I performed a BuildRoot Linux build on an Ubuntu PC.
```
git clone https://github.com/m5stack/CoreMP135_buildroot.git
git clone -b upstream-backport https://github.com/MeemeeLab/CoreMP135_buildroot-external-st.git
cd CoreMP135_buildroot
make BR2_EXTERNAL=../CoreMP135_buildroot-external-st/ m5stack_coremp135_defconfig
make -j4
```
