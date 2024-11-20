# How to disable the intel management engine in Intel Thinkpads?

My device is "21JK0006TX ThinkPad E14 Gen 5".

My UEFI BIOS version is 1.31

My **ME FIRMWARE VERSION** is 16.1.25.2091

- Enter to UEFI BIOS settings
- Disable secure boot first
- Then, completly disable the security chip (TPM)
- Enable all the three options in the virtualization (*it might not be directly related but i am not sure*)
- Finally, permanently disable the Absolute Persistance
- (reboot)
- run the intelmetool, your output should be like:


$ sudo ./intelmetool -m

Can't find ME PCI device

