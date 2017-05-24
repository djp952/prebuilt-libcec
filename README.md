# LIBCEC 4.0.2
[https://github.com/Pulse-Eight/libcec](https://github.com/Pulse-Eight/libcec)  
libCEC(R) is Copyright (C) 2011-2015 Pulse-Eight Limited.  All rights reserved.    
  
**BUILD ENVIRONMENT**  
* Windows 10 x64 15063   
* Visual Studio 2017 (with VC++ 2015.3 v140 toolset and Windows 8.1 SDK)   
  
Open "Developer Command Prompt for VS2017"   
```
git clone https://github.com/Pulse-Eight/libcec -b libcec-4.0.2
cd libcec
git submodule update --init
cd src\platform
notepad .gitmodules
> Replace "git@github.com:" with "https://github.com/"
git submodule update --init
cd ..\..\windows
notepad build.cmd
> Replace "SET VSVERSION=12" with "SET VSVERSION=14"
build
```
