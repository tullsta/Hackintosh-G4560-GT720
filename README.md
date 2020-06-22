# Hackintosh-G4560-GT720 
Hackintosh High Sierra Build How to for G4560 ASUS motherboard and Nvidia GT720 graphic card


# Before start
The best way to clean install is to use whole disc for OSX.
You need to create EFI partition, with minimum size 300MB. You can do it under Windows CMD with discpart tool. 

Type diskpart in CMD terminal.
At the DISKPART prompt, type list disk. Note the disk number that you want to delete.
At the DISKPART prompt, type select disk <disknumber>.
At the DISKPART prompt, type clean.
Important
Running the clean command will delete all partitions or volumes on the disk.
At the DISKPART prompt, type convert gpt
create partition efi size=300M
exit
  

  
# Bdutility

# UEFI 
Reset Bios/Uefi values to default
Change boot priority to start from USB pendrive
Don't use USB 3.0 port for instalation, only USB2!







