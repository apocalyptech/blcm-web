---
permalink: /bl3-running-mods/
---
# Borderlands 3 General Modding Information

Modding in Borderlands 3 is a bit different from how you might be used to dealing
with mods in BL2/TPS.  You will *not* be using BLCMM to manage your mod list, and
you won't be using a console to run any `exec` commands.

Instead, BL3 modding requires that a program modifies the hotfixes that are being
sent from Gearbox, and so another program has to get in the way and do that.  This
is where [B3HM](https://www.nexusmods.com/borderlands3/mods/244) (Borderlands 3
Hotfix Merger) comes in!

# B3HM (Borderlands 3 Hotfix Merger)

B3HM is a tool written by c0dycode to merge in custom hotfixes for BL3 to pick up.
It's available either as a standalone EXE, or as a DLL which you can inject in
a variety of methods.  You can find B3HM in these locations:

- [B3HM at Nexusmods](https://www.nexusmods.com/borderlands3/mods/244)
- [B3HM at Github Releases](https://github.com/c0dycode/BL3HotfixWebUI/releases)

The B3HM project has [documentation right at its github page](https://github.com/c0dycode/BL3HotfixWebUI/wiki/B3HM-Wiki).

For the DLL version, it's recommended that you use
[FromDarkHell's BL3DX11Injection](https://github.com/FromDarkHell/BL3DX11Injection/releases)
to inject the B3HM into the Borderlands 3 process.  For the EXE version, just
download the EXE and give it a run.

See the [B3HM documentation](https://github.com/c0dycode/BL3HotfixWebUI/wiki/B3HM-Wiki) for
further information about how to use the app!

# Finding Mods

Right now, most available BL3 Hotfix mods are being distributed over Github,
similar to how "traditional" BL2/TPS mods have been released in the past.
The *easiest* way to find mods is by using the [BL3 ModCabinet Wiki](https://github.com/BLCM/bl3mods/wiki).

## BL3 ModCabinet Wiki

The [BL3 ModCabinet Wiki](https://github.com/BLCM/bl3mods/wiki) organizes all
the BL3 mods in the main github into categories which should be pretty easy
to click around to find what you're looking for.  For instance, you could click on
"Cheat Mods" on that page to arrive at the
[Movement Speed Cheats Extreme Improvements](https://github.com/BLCM/bl3mods/wiki/Movement%20Speed%20Cheats%20-%20Extreme%20Improvements)
mod, which improves character speed by quite a lot.  From there, you'll see a header
which looks like this:

[![ModCabinet Header](/img/bl3modcabinet.png)](/img/bl3modcabinet.png)

To download the mod to your hard drive, you can right-click on the `Download from Github`
link and choose "Save Link As."  B3HM does not require you to download the mod,
if you don't want to, though!  You could instead right-click on `Download from Github`
and choose "Copy Link Location", and then add in that URL to B3HM's mod list.  That
way you'll always end up loading the most recent version of the mod.

If you want to keep your collection of mods a little more stable, you might want to
download the files locally anyway, of course.

## Direct Github Access

You can also download BL3 mods directly from [the bl3mods Github page](https://github.com/BLCM/bl3mods),
though they will be organized by author, rather than category.
When you browse to a `.bl3hotfix` mod file you want to download, it will either
have a `Raw` button or a `Download` button, in the upper right hand corner of the
file's contents:

[![Raw Button](/img/github_raw.png)](/img/github_raw.png)

[![Download Button](/img/github_download.png)](/img/github_download.png)

Right-click on that button and choose `Save Link As...` to save the file to
your computer, or `Copy Link Location` to import it as a URL into B3HM instead.

# Info for Linux Users

Borderlands 3 doesn't have a native Linux version, but Linux users have been
able to [run BL3 via proton](https://www.protondb.com/app/397540) for some
time now.  Unfortunately, with the limited testing done so far, we've not had
much success getting B3HM running in that environment.

Fortunately for Linux users, there's an alternate method which has been available
for some time now, although it requires quite a bit more manual setup than
B3HM does.  Check out [apocalyptech's bl3hotfixmodding repo](https://github.com/apocalyptech/bl3hotfixmodding)
for a general overview of the technique, and a [mitmproxy](https://mitmproxy.org/)-based
script to handle loading mods and getting the hotfix injection working right.
That page doesn't go into *all* the details necessary to get mitmproxy up and
running for this purpose, but feel free to ask apocalyptech about it in
[Shadow's Evil Hideout](https://discord.gg/shadowevil).

