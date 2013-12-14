Fentanyl
========

An IDAPython script that makes patching significantly easier. Fentanyl lets you patch from IDA Pro or Demo easily. Most patches can be done without touching a hex editor but if you must edit raw bytes you can simply use IDA's hex view. You can also undo and redo changes to the idb. 

For context menu options install Python 2.6, use the respective IDAPython version, and download the PySide bindings below. 
IDAPython: https://code.google.com/p/idapython/

IDA PySide: http://dvlabs.tippingpoint.com/img/mindshare/PySide-1.0.8qt473.win32-py2.6.exe

Helfpul if you want to run scripts on startup: https://code.google.com/p/idapython/source/browse/trunk/examples/idapythonrc.py

Alt F7 to load scripts

File > Produce file > Create DIF file
Edit > Patch program > Apply patches to input file

Right click bytes in hex view and click edit to begin editting. 
Right click again and select Apply Changes to save changes. 

Keybindings:
 * Shift-N: Convert instructions to nops
 * Shift-X: Nop all xrefs to this function
 * Shift-J: Invert conditional jump
 * Shift-U: Make jump unconditional
 * Shift-P: Patch instruction
 * Shift-Z: Undo modification (Won't always work. Should still be careful editing.)
 * Shift-Y: Redo modification (Won't always work. Should still be careful editing.)
 * Shift-S: Save file
