# How to install Touhou with English patches
## Acquire the Games
You can acquire the games digitally from:
 * [Steam](https://store.steampowered.com/search/?developer=%E4%B8%8A%E6%B5%B7%E3%82%A2%E3%83%AA%E3%82%B9%E5%B9%BB%E6%A8%82%E5%9B%A3) (Not recommended due to Steam DRM sometimes present),
 * [DLSite](https://www.dlsite.com/home/dlaf/=/aid/tudi20/url/https%3A%2F%2Fwww.dlsite.com%2Feng%2Fcircle%2Fprofile%2F%3D%2Fmaker_id%2FRG46179.html%2F%3Futm_medium%3Daffiliate%26utm_campaign%3Dbnlink%26utm_content%3Dtext) (Affiliate Link),

 * Piracy sites (recommended getting one with pre-packed with thpatch then) only use as last resort, SUPPORT CREATORS.
 
For physical copies see [Touhou Wiki's Purhcasing Guide](https://en.touhouwiki.net/wiki/Purchasing_Guide) for information.
 
## Installing thcrap
 * Browse to the folder that contains your Touhou games and remember it.
   * **Steam:** Go to your installation for Steam, right-click on your game in the client, select Manage and then Browse local files.
   * **Other:** Wherever you selected to download/install the game.
 * If you see a thcrap folder you can skip the downloading part.
 * Download [THCRAP](https://www.thpatch.net/wiki/Touhou_Patch_Center:Download), and extract it somewhere close.
 * Run `thcrap-configure.exe`.
 
## Installing the English patch
 * After clicking Next and it is downloading a few files; scroll up and double click on `lang_en`. Click Next.
 * Wait for it to download stuff again >.<.
 * Just accept the default name aka click Next.
 * Next again, and again. _We do really need a new GUI..._
 * Select your Touhou folder (that I made you remember above) in the popped up folder browser.
   >If you have multiple Touhou games, select the folder that contains all of them!
 * After this, grab the right side of the window and extend it, and click on the ones that **DOES NOT** contain `(not recommended)`.
 * After done, click yes.
 * Wait till it downloads the patches. Grab a coffee; if something goes wrong somewhere you might be pulling all-nighter >.<.
 * Click next. You're done!
 * Go click on one of the shortcuts it created and have a go! If you don't like shortcuts, check out the next section:
 
## Optional: Get Universal THCRAP Launcher (aka. UTL) for short
 * Go to [this page](https://github.com/thpatch/Universal-THCRAP-Launcher/releases) and download `utl.rar`.
 * Follow the instructions [here](https://github.com/thpatch/Universal-THCRAP-Launcher#installation).
 
## Optional: Setting up vpatch

### By default
 * Go to [this page](https://www.mediafire.com/file/zxdhr7rdpzrlnmt/VsyncPatch.zip/file) and download it.
 * Extract it and follow the instructions in the provided text file.
   * Which basically is copy the right thing to the right place.
   * You need the `vpatch.exe`, `vpatch.ini`, and the right dll for your game, copied in the game's folder.
   * Note that both rev4 and rev7 has dlls for th10, th11, and th095.
 * Configure the `vpatch.ini` file to your liking. You will probably want to set a few things like actually enabling vsync if you aren't using 60hz monitor, changing the resolution, changing if it should be borderless, or ask if you want it to be full screen or windowed every time, for games that didn't had this functionality.
 * For older games it also ports back some of the newer games' features, like Ctrl skipping in dialogue or replays.
 * You must run `vpatch.exe`.
   >Note: Vpatch will always launch `thxx.exe` or the like (except th06), so if you want it to run the static English patch, you will have to rename those.
  
### Touhou 6 is a bit more janky
 * Since ZUN decided to use Japanese in file names, and Windows XP back then didn't knew what UTF-8 is, unless your system is fully in Japanese, your Touhou 6 won't run, since it doesn't match up with what vpatch except, since your file name is in [mojibake](https://en.wikipedia.org/wiki/Mojibake).
 * You will have to follow instruction about this on [thpatch's site](https://www.thpatch.net/wiki/Touhou_Patch_Center:Download#HALP.21_My_Embodiment_of_Scarlet_Devil_runs_like_a_Tengu_jet_fighter_on_steroids.21.21).
 
### Adding it to thcrap

#### Legacy
 * Go to your thcrap folder, open the `config` folder, and inside it, open `games.js˛` **IN A TEXT EDITOR**.
 * Edit the lines that have paths to your games (usually ending in "thxx.exe"), to and change the "thxx.exe" part to "vpatch.exe".
 * [This is an example file of how your thcrap/config/games.js should look like, if you want to use it with vpatch.](https://gist.github.com/Tudi20/029f63dbc85a838d97ad0fb973956266).
   * Yours will probably need to look different.
 * You can just launch thcrap regularly.
 
#### Modern
 * New thcrap should automatically detect vpatch in the scanning for games part of configuration, so you should just re-run that. Just to be sure choose "Rescan" instead of "Add new games".
 
## Troubleshooting

### "d3dx9_XX.dll not found"
 * Install DirectX 9 from [here](https://www.microsoft.com/en-us/download/details.aspx?id=35).
   
### Touhou 6 runs above 60 fps and is on steroids
 * See the thpatch section on it, [here](https://www.thpatch.net/wiki/Touhou_Patch_Center:Download#HALP.21_My_Embodiment_of_Scarlet_Devil_runs_like_a_Tengu_jet_fighter_on_steroids.21.21).

### Other
 * Something went wrong and not listed here? Oh no! However, you don't need to worry as a bunch of tech monkeys, who got left with the code base mess that an angry German made is available at [THPATCH's Discord server's #support channel](https://discord.thpatch.net/).

## How do I help with the translations?
 That's easy! Just register, and start translating on the [thpatch wiki](https://thpatch.net).
 
## I can code! Can I help?
 Sure! Head over to [THPATCH's Discord server](https://discord.thpatch.net/) and we will sort you out.
 
## I have the money! Where can I donate?
 * [THPATCH](https://opencollective.com/thpatch/),
 * [Me](https://ko-fi.com/tudi20).
 
## How do I make mods?
 That's a bit more complicated... but you can get started by joining the [THPATCH's Discord server](https://discord.thpatch.net/) if you need any help, and reading trough [this](https://gist.github.com/WindowDump/e007516524b7488eccf74a020b3c7977) and at least 1.0 from [this](https://priw8.github.io/#b=ecl-tutorial/&p=1).
