# winxp-efi-loader-collection
some ways to boot winxp/2003 on uefi
1.Quibble(https://github.com/maharmstone/quibble/) MAY be capable of booting both x64 and x86 versions of winxp/2003.
2.boot loader from windows longhorn build 5219 allows x86 version to boot on uefi
howto:
1.Install it(xp only,it's said that 2k3 doesn't work)normally,but make the boot partition fat32.
2.download the file labeled x86.Put the winload.efi in system32.
3.Create folders like this in boot partition:/efi/boot/,put bootia32.efi in boot.
4.remove the read-only attribute of boot.ini and add /NOBCD /USENEWLOADER options,save boot.ini.
5.use uefi firmware to try to boot it and wish that it works.
