# Riru-Il2CppDumper
Riru's version of Il2CppDumper, used to bypass protection, encryption, and obfuscation by dumping data while the game is running.

## How to use
1. install [Magisk](https://github.com/topjohnwu/Magisk) and [Riru](https://github.com/RikkaApps/Riru).
2. download source code
Edit `game.h`, modify the game package name `GamePackageName` and the Unity version `UnityVersion`.
4. run the gradle task `:module:assemblyRelease` compiled using Android Studio
Install the module in Magisk.
6. start the game and generate `dump.cs` in `/data/data/GamePackageName/files/`.

## TODO
- [x] Lower versions use reflections for dumping
- [x] Higher versions use `il2cpp_image_get_class` for dumping.
- [ ] Refine the dump.cs output
- [ ] Generic Correlation Output
- [ ] Generating IDA Scripts
- [ ] generating header files
