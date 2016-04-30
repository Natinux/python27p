# python27p
Single-File Stand-alone Python 2.7.9 for Windows

Taken from [orbitals](http://www.orbitals.com/programs/pyexe.html)

`py.exe` - Python 2.7.9 as a single, stand-alone executable with virtually all the standard libraries, plus pywin32-219 and psutil 2.1.3. Compiled with py2exe (see source below) on Windows XP. This should work on Windows XP and later. This works just like a full install of python, except you only need the one file. 9.9 Mb.

`pyexe-2.7.9.10.zip` - Zip file of the stand-alone exectuable. 9.8 Mb.

`pyexe-src-2.7.9.10.zip` - The source code for making the py.exe file. See the README.TXT within the zip file for details. Requires a full install Python 2.7.9, pywin32-219, psutil 2.1.3, setuptools.py, and py2exe. 10 kb.

# Rationale 

I frequently write programs in python as it is a handy, powerful language. However, sometimes I don't want to install it. There are some other projects to give a portable python implementation. That still seems too heavy for some tasks.

Here is a Windows executable form of Python 2.7.9 that contains most of the standard libraries, plus pywin32. It has the following features:

* Single file with no dependencies besides Windows (XP or later)
* Can run python programs (e.g., py.exe sample_program.py)
* Can be used as an interactive shell (e.g., py.exe, then start typing)
* Can be used to execute string commands (e.g., py.exe -c "print 'hello world'")
I've included the very simple source code, which is nothing more than a setup.py script using py2exe. I compressed the executable using upx, which reduces its size by 12% or so and doesn't substantially slow down starting the program.

Note: I have one report that when running the program on Windows 7 64-bit, you need to have the current working directory set to the location of the py.exe program. Not having a copy of Windows 7 64 bit, I cannot determine if I could work around this issue.

2013 May 19 - David Manthey - Updated 2015 January 4
