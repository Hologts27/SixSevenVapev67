<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./README/vapelogo-white.png">
    <source media="(prefers-color-scheme: light)" srcset="./README/vapelogo-dark.png">
    <img alt="vape logo" src="./README/vapelogo.png">
  </picture>
</p>
<h2 align="center">
  A highly optimized and stable fork of the legendary Vape V4!
  <br/>
  Rise up to the top while remaining completely untouchable and crash-free.
</h2>

---

## 🚀 Improvements & Stability Fixes
This version (SixSevenVapev67) focuses on resolving critical stability issues present in the original repository, specifically targeting frequent crashes and performance bottlenecks.

- **Permanent Hooking System**: Replaced the unstable hook/unhook cycle with a permanent gating system. This prevents fatal client crashes when rapidly toggling modules like Silent Aim.
- **NaN Vector Protection**: Hardened mathematics in raycasting logic to prevent "Division by Zero" errors (NaN vectors), which are the #1 cause of sudden game closes.
- **Thread Leak Prevention**: Optimized execution loops to ensure that toggling modules doesn't leave behind "zombie threads," preserving your CPU performance for the game.
- **Enhanced Executor Support**: Replaced direct focus calls with a safer detector, ensuring compatibility with executors that handle `iswindowactive` as a boolean.
- **Validation Layers**: Added recursive instance checks for Target parts to prevent "Nil Access" errors during high-speed combat.

## Usage
1. Download a high-quality scripting utility for Roblox.
2. Execute the provided loadstring below.
```luau
loadstring(game:HttpGet("https://raw.githubusercontent.com/Hologts27/SixSevenVapev67/main/NewMainScript.lua", true))()
```

## Troubleshooting
If you encounter issues, please try these steps:
1. **Delete the `newvape` folder** (with the game closed) to clear cached old files.
2. Ensure your executor supports **file functions** and the **debug library**.
3. Making sure you have connection to [the main loadstring.](https://raw.githubusercontent.com/Hologts27/SixSevenVapev67/refs/heads/main/NewMainScript.lua)

## Developers & Credits
- **Original Lead**: [7GrandDad](https://github.com/7GrandDadPGN) - Lead maintainer of the project - vaperoblox on Discord.
- **Refinement & Stability**: [Hologts27](https://github.com/Hologts27) - Performance optimizations and crash-prevention patches.
- **bytecode disassembly**: [rce-incorporated](https://github.com/rce-incorporated/Fiu)
- **HashLibrary**: [Egor Skriptunoff, boatbomber, and howmanysmall](https://devforum.roblox.com/t/open-source-hashlib/416732/1)
- **Projectile Prediction**: [Vernumerator](https://devforum.roblox.com/t/predict-projectile-ballistics-including-gravity-and-motion/1842434)

---
<p align="center">Made for the community, by the community.</p>
