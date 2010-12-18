bootloader-18f
==============

This contains a modified version of the tiny bootloader, modified to
make it more robust and hence more suitable for use in devices that
will be reprogrammed "in field".

The license is the same as tinybld, specifically:

"you can modify the PIC source files for your purposes, but don't forget
to mention the original source of inspiration and the author."

Please see here for the original:

http://www.etc.ugal.ro/cchiculita/software/picbootloader.htm



pc-software
===========

Contains a command line application to talk to the bootloader. As the
protocol has not changed, this software can also be used with the
unmodified tiny bootloader if desired. (The tiny bootloader PC app is
written in Delphi and available on Windows only; this one is written in
pure C and is also available for linux.)

Three build environments are supported:

linux: type "make"

Microsoft Visual VC++ 6: use bootloader.dsp

Microsoft Visual Studio 2005: use bootloader.sln


The firmware image can be embedded into the binary using the
encodefirmware.pl perl script.


The license can be found in pc-software/LICENSE.txt

If you don't like the license feel free to ask, I'll probably let you
use it under a different license.



--

Joseph Heenan, December 2010
joseph@heenan.me.uk
http://code.google.com/p/pic-bootloaders/
