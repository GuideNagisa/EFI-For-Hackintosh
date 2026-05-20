# Intel Core i7 6700 + IGPU Intel HD 530 (Skylake) Fix IGPU 7MB to 1536 MB

<img width="753" height="501" alt="Screen Shot 2569-05-21 at 00 11 49" src="https://github.com/user-attachments/assets/a609d327-20e5-4626-b43d-5a4c23d62594" />

Test on MacOS Monterey / Bigsur it's Work Fine!

- Use OpenCore Configutator / OCAuxiliaryTools

* DeviceProperties
  PciRoot(0x0)/Pci(0x2,0x0) - AAPL,ig-platform-id / 00001219 / DATA
                            - device-id / 12190000 / DATA

* NVRAM
  7C436110-AB2A-4BBB-A880-FE41995C9F82 - boot-args / -v keepsyms=1 debug=0x100 alcid=1 -igfxonlnfb -disablegfxfirmware / STRING
                                       - csr-active-config / 030A0000 / DATA

- Use OCAuxiliaryTools
  Check for kexts Updates / Start Sync (Check it's All Green)
  - SAVE And RESTART / Reset NVRAM
 
All Done! 
