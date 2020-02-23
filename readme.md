Instructions:
1. Format USB with EFI and Boot files
2. Edit config.plist file using updated configuration (Line 18)
3. Use GenSMBIOS and macinfo to update all keys

GenSMBIOS Instructions
1. Run GenSMBIOS.bat file
2. Enter 4 for UUID
3. Replace all cases of UUID in config.plist with new ID
	Note: Use control+f to navigate to "Data Hub"

MacInfo Instructions
1. Navigate to macserial32.exe in CMD with admin privileges
2. once inside macinfo folder enter: macserial32.exe -h to see
   options
3. for this case will enter : macserial32.exe --model iMacPro1,1
4. Replace all generated casses of UUID in config.plist with new ID
	Note: Use control+f to navigate to "Data Hub"

Patches.plist Instructions
1. Copy Patch from <array> to </array> 
	In this case it would start at line 82 and end at 1235
2. Paste into your config.plist file, making sure to only edit the
	patches array