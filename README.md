# Welcome to the FamiStudio GitHub page
This is the GitHub page of FamiStudio, which is intended for people wanting to view/download the source code or report bug fixes.

**If you are simply interested in installing FamiStudio, please visit the brand new [famistudio.org](https://famistudio.org/) or [itch.io](https://bleubleu.itch.io/famistudio).**

For any questions, you can reach me at [famistudio@outlook.com](mailto:famistudio@outlook.com).

## Compiled versions
All releases are available in the [Releases](https://github.com/BleuBleu/FamiStudio/releases) section. If you are on Windows, simply download and run the .MSI installer and a shortcut to FamiStudio will be placed in your Start menu.

## Compiling
The tools needed to compile are:
- Visual Studio 2017 on Windows 
- Visual Studio 2019 for Mac, on MacOS
- MonoDevelop on Linux, I use 7.8.4 (build 2) (the Linux version is not usable, but it should compile, launch and play a song)

FamiStudio is composed of a few projects:
- The main FamiStudio application is written in C#. 
- NesSndEmu & NotSoFatso are C++ DLLs and are provided as binaries since they rarely change. In you plan to recompile them, you will need to install C++ support in Visual Studio. On MacOS and Linux, there is a small build shell script included.
- The Setup project (Windows-only) is built using the "Microsoft Visual Studio Installer Projects" extension which can be installed from Visual Studio in the "Extensions and Updates" menu.

The C# application is built on top of SharpDX 4.2.0 on Windows and OpenTK on Mac/Linux. Visual Studio will install the required packages automatically when building the project. To manually fetch the packages, run `msbuild /t:Restore` on the project from the Visual Studio Developer Command Prompt.

## Issues and Contributing
Please open issues contact me if you find bugs or have feature suggestion ideas. 
You can find me:
- On the [NESDEV Forums](https://forums.nesdev.com/) as BleuBleu 
- On Twitter [@NesBleuBleu](http://www.twitter.com/nesbleubleu)
- On [YouTube](https://www.youtube.com/channel/UC-dGLo2XZqXNA_aOYjaucgA?view_as=subscriber)
- On [Itch.io](https://bleubleu.itch.io/famistudio)

## Acknowledgments
- [Shiru](https://shiru.untergrund.net/code.shtml) for the FamiTone2 library and the demo songs that are included (_After the Rain_ and _Danger Streets_)
- [Blargg](http://www.slack.net/~ant/) for Nes_Snd_Emu and the underlying Blip_Buffer. Also for it's Smooth Vibrato tech.
- [RainWarrior](http://rainwarrior.ca) for NSFImport and other tools.
- [Mitsutaka Okazaki](https://github.com/okaxaki) For emu2413 and emu2149 which are used for VRC7 and Sunsoft 5B emulation.

