# Setup

Addionally to the compiler, found [here](https://github.com/jeanpmathes/ance), multiple environment variables and directories have to be set up. 

## ANCE_PACKAGE_DIRECTORY 

In this directory, all packages are searched.
To use ance, clone [std](https://github.com/ance-lang/std) and [project](https://github.com/ance-lang/project) into this directory.
This is where you should create your own projects. 

## ANCE_RESOURCE_DATA_DIRECTORY

This directory contains required resources like the ance-specific runtime.
Unpack the newest release of the [runtime](https://github.com/ance-lang/runtime) into the target directory of this directory.
The resulting structure should look like this:

```
ANCE_RESOURCE_DATA_DIRECTORY/
├─ targets/
│  ├─ x86_64-pc-windows-msvc/
│  │  ├─ runtime.dll
│  │  ├─ runtime.lib

```

## ANCE_SYSTEM_RUNTIME_DIRECTORY

This directory contains the C runtime of your operating system. 
On windows, install MSVC using Visual Studio and select the appropriate directory there.

## ANCE_SYSTEM_SDK_DIRECTORY

This directory contains your OS SDK, on windows this would be the library directory of your Windows Kit. 

# Programming 

Refer to the [hello_world](https://github.com/ance-lang/hello_world) project to see the basic structure.
To compile, use `ance.exe hello_world.ance`.
To execute, find the executable in the `bld/<target>/bin/` directory.

