simple_av
=========

Simple AV avoiding infections through removable media.
The tools performs a fast scan when the media is connected, then asks the user for a complete scan.

Detection engine is based on :
- MD5 hash database (if a file is detected, it is removed)
- filesystem's attributes (hidden, system and readonly. If a file is detected, it is renamed)
- autorun.inf (if detected, disabled by renaming to autorun.inf and targeted binary is also renamed).

The suspected files are renamed from file.exe to file.exe.vir.

Coded for personal usage and fun.
