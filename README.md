Spell Revisions aims to fix, tweak, and enhance arcane and divine spells in Baldur's Gate II, either the classical or the enhanced editions, including [BGT](https://github.com/SpellholdStudios/BGT-WeiDU) and [EET](https://github.com/Gibberlings3/EET).

The mod comes with documentation that you can find [here](./readme-spell_rev.html). Detailed lists of spells can be consulted [here](https://gibberlings3.github.io/SpellRevisions/).

note(s):
- The spell documentation, both the one shipped with the mod and the one in [GitHub](https://gibberlings3.github.io/SpellRevisions/), has *not* been updated to reflect the changes since the 4.18beta. The in-game documentation is of course, fully up dated.

# A. Latest release.

Latest release is 4.19rc5.

From the github page, click on releases in the side-bar to download it. If you are feeling *really* adventurous, then you can download the absolute latest by clicking on the code button and then downloading the zip.

Note that it is a *source release*; it just bundles the files in the GitHub repository in an archive and does not have any executables, so for the installation you will need the command line -- see section below. It is slightly more inconvenient for users than the standard release, but it allows for faster and more timely releases.

# B. Installation.

Installation is like any other WeiDU mod -- see [A New Player’s Guide to Installing and Playing Mods](https://www.gibberlings3.net/forums/topic/33164-a-new-player%E2%80%99s-guide-to-installing-and-playing-mods/).

## B. 1. Command line.

Assuming you have WeiDU [^1] installed and on the executable path [^2], just download the release zip file, unzip it with whatever archive unzipper your platform supports into some temporary location, and copy the folder [^3] `spell_rev` to your Baldur's Gate install directory. Then open a command line, change directory to the BG installation dir and do

```
weinstall spell_rev
```

and install the components you want.

## B. 2. Double-clicking.

If the command line is proving to be too difficult (e.g. Windows platform, do not have `weinstall` in the executable path, etc.), you can install as usual by double clicking the executable installer. For a *source release* that does not come with an executable installer, you can proceed as follows:

* Do the same download, copy into BG installation dir, etc. as in previous point B. 1. 
* Download any, relatively recent updated, mod with such an installer, e.g. [Tweaks Anthology](https://www.gibberlings3.net/files/file/973-the-tweaks-anthology/).
* Grab its executable installer, rename it as `setup-spell_rev.exe` and drop it on the root dir of `spell_rev`.
* Double-click the executable and proceed as usual.

[^1]: latest version can be grabbed from [here](https://github.com/WeiDUorg/weidu/releases).

[^2]: precise details depend on the platform.

[^3]: for a source release, the top folder is *not* what one wants, rather it is the `spell_rev` subfolder.

# C. Mod order.

For general advice on install order, you can consult various submitted mod load orders at [Baldur's Gate Install Order List Repository](https://github.com/morpheus562/Baldurs-Gate-Install-Order-List-Repository).

SR's main component does wholesale spell replacement, so it should be installed relatively early in the install order, certainly before Tweaks Anthology and SCS. On the other hand the "Update NPC spellbooks" component should be installed after all NPC mods.
