# Alchemy XP Fix

Award XP for learning ingredient effects when creating potions

## Requirements
* [CMake](https://cmake.org/)
	* Add this to your `PATH`
* [PowerShell](https://github.com/PowerShell/PowerShell/releases/latest)
* [Vcpkg](https://github.com/microsoft/vcpkg)
	* Add the environment variable `VCPKG_ROOT` with the value as the path to the folder containing vcpkg
* [Visual Studio Community 2022](https://visualstudio.microsoft.com/)
	* Desktop development with C++
* [CommonLibSSE](https://github.com/powerof3/CommonLibSSE/tree/dev) (For SE/AE)
	* You need to build from the powerof3/dev branch
	* Add this as as an environment variable `CommonLibSSEPath`
* [CommonLibVR](https://github.com/RafearTheModder/CommonLibVR/tree/vr) (For VR)
	* You need to build from the RafearTheModder/vr branch
	* Add this as as an environment variable `CommonLibVRPath`

## User Requirements
* [Address Library for SKSE](https://www.nexusmods.com/skyrimspecialedition/mods/32444)
	* Needed for SSE/AE

## Register Visual Studio as a Generator
* Open `x64 Native Tools Command Prompt`
* Run `cmake`
* Close the cmd window

## Building
```
git clone https://github.com/powerof3/AlchemyXPFix.git
cd AlchemyXPFix
```

### SSE
```
cmake --preset vs2022-windows-vcpkg-se
cmake --build build --config Release
```
### AE
```
cmake --preset vs2022-windows-vcpkg-ae
cmake --build buildae --config Release
```
### VR
```
cmake --preset vs2022-windows-vcpkg-vr
cmake --build buildvr --config Release
```
## License
[MIT](LICENSE)
