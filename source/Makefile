# AutoHotkey.exe: AutoHotkey.o Script.o script2.o script_object.o SimpleHeap.o StringConv.o TextIO.o
AutoHotkey.exe: AutoHotkey.o
	gcc $^ -o $@

AutoHotkey.o: AutoHotkey.cpp stdafx.h globaldata.h hook.h hotkey.h \
 keyboard_mouse.h defines.h ahkversion.h script.h SimpleHeap.h var.h \
 clipboard.h util.h WinGroup.h Util.h resources/resource.h \
 script_object.h Debugger.h os_version.h application.h window.h TextIO.h
	gcc $(COPTS) -Wno-write-strings -fpermissive $< -c -o $@

Script.o: Script.cpp stdafx.h config.h debug.h KuString.h StringConv.h \
 script.h defines.h ahkversion.h SimpleHeap.h keyboard_mouse.h var.h \
 clipboard.h util.h WinGroup.h Util.h resources/resource.h \
 script_object.h Debugger.h os_version.h globaldata.h hook.h hotkey.h \
 mt19937ar-cok.h window.h application.h TextIO.h
	gcc $(COPTS) -Wno-write-strings -fpermissive $< -c -o $@

script2.o: script2.cpp stdafx.h config.h debug.h KuString.h StringConv.h \
 qmath.h mt19937ar-cok.h script.h defines.h ahkversion.h SimpleHeap.h \
 keyboard_mouse.h var.h clipboard.h util.h WinGroup.h Util.h \
 resources/resource.h script_object.h Debugger.h os_version.h window.h \
 globaldata.h hook.h hotkey.h application.h TextIO.h lib_pcre/pcre/pcre.h \
 lib_pcre/pcre/pcret.h script_func_impl.h
	gcc $(COPTS) -Wno-write-strings -fpermissive $< -c -o $@

script_object.o: script_object.cpp stdafx.h config.h debug.h KuString.h \
 StringConv.h defines.h ahkversion.h globaldata.h hook.h hotkey.h \
 keyboard_mouse.h script.h SimpleHeap.h var.h clipboard.h util.h \
 WinGroup.h Util.h resources/resource.h script_object.h Debugger.h \
 os_version.h application.h script_func_impl.h
	gcc $(COPTS) -Wno-write-strings -fpermissive $< -c -o $@

SimpleHeap.o: SimpleHeap.cpp stdafx.h config.h debug.h KuString.h \
 StringConv.h SimpleHeap.h globaldata.h hook.h hotkey.h keyboard_mouse.h \
 defines.h ahkversion.h script.h var.h clipboard.h util.h WinGroup.h \
 Util.h resources/resource.h script_object.h Debugger.h os_version.h
	gcc $(COPTS) -Wno-write-strings -fpermissive $< -c -o $@

StringConv.o: StringConv.cpp stdafx.h config.h debug.h KuString.h \
 StringConv.h util.h defines.h ahkversion.h
	gcc $(COPTS) -Wno-write-strings -fpermissive $< -c -o $@

TextIO.o: TextIO.cpp stdafx.h config.h debug.h KuString.h StringConv.h \
 TextIO.h script.h defines.h ahkversion.h SimpleHeap.h keyboard_mouse.h \
 var.h clipboard.h util.h WinGroup.h Util.h resources/resource.h \
 script_object.h Debugger.h os_version.h script_func_impl.h
	gcc $(COPTS) -Wno-write-strings -fpermissive $< -c -o $@
