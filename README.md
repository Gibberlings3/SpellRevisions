Spell Revisions aims to fix, tweak, and enhance arcane and divine spells in Baldur's Gate II, either the classical or the enhanced editions, including [BGT](https://github.com/SpellholdStudios/BGT-WeiDU) and [EET](https://github.com/Gibberlings3/EET).

The mod comes with documentation that you can find [here](./readme-spell_rev.html). Detailed lists of spells can be consulted [here](https://gibberlings3.github.io/SpellRevisions/).

# A. Latest release.

Latest release is 4.19rc1.

It is a *source release*; it just bundles the files in the GitHub repository in an archive. It is slightly more inconvenient for users than the standard release, but it allows for faster and more timely releases.

# B. Installation.

Installation is like any other WeiDU mod. Download the release zip file, unzip it with whatever archive unzipper your platform supports into some temporary location, and copy the folder [1^] `spell_rev` to your Baldur's Gate install directory. Then do

```
weinstall spell_rev
```

and install the components you want.

[1^] for a source release, the top folder is *not* what one wants, rather it is the `spell_rev` subfolder.

# C. Mod order.

For general advice on install order, you can consult various submitted mod load orders at [Baldur's Gate Install Order List Repository](https://github.com/morpheus562/Baldurs-Gate-Install-Order-List-Repository).

SR's main component does wholesale spell replacement, so it should be installed relatively early in the install order, certainly before Tweaks Anthology and SCS. On the other hand the "Update NPC spellbooks" component should be installed after all NPC mods.
