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
  

  
# Bdutility - http://cvad-mac.narod.ru/index/bootdiskutility_exe/0-5
Download BootDisk Utility, and install it.

You need at lease 4GB USB drive
1. Press Format - this will create 2 partitions on the USB drive
2. Press DL Center, choose High Sierra Recovery HD and click Download (DL)
3. The proigram will save new hfs file in the folder.
4. Select empty partition (not Clover) in the program, click Restore, and choose hfs file from previous step
5. After installing press Eject
Mount the USB drive once again.

Now download EFI folder from this repository, and replace all the files on USB drive Clover partition
EFI filder contains all files needed to boot OSX with Clover. 

# UEFI 
Reset Bios/Uefi values to default
Change boot priority to start from USB pendrive
Don't use USB 3.0 port for instalation, only USB2!







