# A. Changelog.

## Version: 4.21 -- unreleased.

1. [Fix bg1 ee strings](https://github.com/Gibberlings3/SpellRevisions/pull/153): patch by aigleborgne, with help of jmerry over at the G3 forums, to fix wrong strings being displayed in bg1 ee. Thanks to them both.

## Version: 4.20.

1. [Fix iwd install](https://github.com/Gibberlings3/SpellRevisions/pull/151): fixes several issues that made the installation in iwd ee fail. See the PR for more details.

## Version: 4.19.

The highlight of this new version is in the purely administrative side of leaving beta status behind and adding a readme to the GitHub site and a brand new spanking changelog in markdown, which you are now reading. Very little in terms of new features, most of the changes are in polishing old code (of which there is a lot) and bug fixes.

The most salient ones are:

1. [Fix icons for Obscuring Mist and Monster Summoning I scrolls](https://github.com/Gibberlings3/SpellRevisions/pull/25)
2. [Fix compatibility issue with DR v8+](https://github.com/Gibberlings3/SpellRevisions/pull/40)
3. Spell fixes. Too many to document here, so we just link to the respective PR's for the documentation.

   * [Arcane level 1 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/41)
   * [Arcane level 2 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/47)
   * [Arcane level 3 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/49)
   * [Arcane level 4 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/51)
   * [Arcane level 5 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/53)
   * [Arcane level 6 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/56)
   * [Arcane level 7 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/58)
   * [Arcane level 8 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/61)
   * [Arcane level 9 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/63)
   * [Divine level 1 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/46)
   * [Divine level 2 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/48)
   * [Divine level 3 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/50)
   * [Divine level 4 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/52)
   * [Divine level 5 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/54)
   * [Divine level 6 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/57)
   * [Divine level 7 Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/59)
   * [Incorrect patching](https://github.com/Gibberlings3/SpellRevisions/pull/67)
   * [More Spell Fixes](https://github.com/Gibberlings3/SpellRevisions/pull/74)

4. [Update spell school setting code](https://github.com/Gibberlings3/SpellRevisions/pull/42)
5. [Update nwn-like spell deflection code](https://github.com/Gibberlings3/SpellRevisions/pull/43)
6. [Update Haste + Slow patching code](https://github.com/Gibberlings3/SpellRevisions/pull/44)
7. [Handling of some IR items](https://github.com/Gibberlings3/SpellRevisions/pull/45)
8. [RFC:Greater Malison](https://github.com/Gibberlings3/SpellRevisions/pull/55)
9. [RFC:Neutral Charm Spells](https://github.com/Gibberlings3/SpellRevisions/pull/64)
10. [Patch to Fire Shield protection from insects](https://github.com/Gibberlings3/SpellRevisions/pull/66)
11. [Update description of Non-Detection](https://github.com/Gibberlings3/SpellRevisions/pull/71)
12. [RFC: Prismatic Mantle](https://github.com/Gibberlings3/SpellRevisions/pull/72)
13. Spell flags: a series of patches that allows users (and developers short on time) to fiddle with spell flags like break invisibility, hostile, etc. The first was [Invisibility and Hostile flags](https://github.com/Gibberlings3/SpellRevisions/pull/73), based on subtledoctor's work, the second, [Three-state flags](https://github.com/Gibberlings3/SpellRevisions/pull/84), allowed to clear the flags (i.e. set to 0), and the third, [Add more spell flags](https://github.com/Gibberlings3/SpellRevisions/pull/88), extended the ability to other spell flags like non-combat. At the moment, only the flags break invisible and hostile have meaningful set values, but these themselves need to be combed over.
14. [Re-write and bug-fix EE refresh, non-stacking code](https://github.com/Gibberlings3/SpellRevisions/pull/75)
15. [Drop concentration checks](https://github.com/Gibberlings3/SpellRevisions/pull/81): the formula for concentration checks is bugged, so until Beamdog fixes it, reverting to vanilla behavior.
16. [Berserk -> Feeblemind in Chaos](https://github.com/Gibberlings3/SpellRevisions/pull/87): The Berserk opcode does not work correctly on non-party members in old, non-EE BG versions, so it was decided to change the Chaos spells to inflict feeblemind instead.
17. [Avenger Cone of Cold -> Confusion](https://github.com/Gibberlings3/SpellRevisions/pull/90): SR changes the level 4 Avenger spell from Chaos to Cone of Cold. There is something to be said about this choice, but it has its downsides, not the least confusing SCS (in fairness, in part because it was implemented as a straight override) so it was decided to switch back to a spell that is closer to the original Chaos.
18. [Fix dvbanish](https://github.com/Gibberlings3/SpellRevisions/pull/92)
19. [French translation](https://github.com/Gibberlings3/SpellRevisions/pull/93): French translation files generously provided by mleduque.
20. [Fix Shapechange ability names in IWD](https://github.com/Gibberlings3/SpellRevisions/pull/96): Patch by gsz. Then improved in [Extract spirit troll shapechange name and add FR translation](https://github.com/Gibberlings3/SpellRevisions/pull/105) by mleduque.
21. [Power level fix on Vitriolic Sphere](https://github.com/Gibberlings3/SpellRevisions/pull/98): Power Level on Vitriolic Sphere acid damage opcode -> 4. Patch by Bartimeus.
22. [LABEL components](https://github.com/Gibberlings3/SpellRevisions/pull/100): Add `LABEL` commands to every (non-deprecated) component.
23. [Fix displayed strings in spells](https://github.com/Gibberlings3/SpellRevisions/pull/107): Improved in [Fix Ray Enfeeble message (and overall improvements)](https://github.com/Gibberlings3/SpellRevisions/pull/134).
24. [Fixes to Elemental Prince HLA](https://github.com/Gibberlings3/SpellRevisions/pull/114):
25. [Missing projectile in Avenger's chromatic orb](https://github.com/Gibberlings3/SpellRevisions/pull/117): patch by mercurier.
26. [Patching hidespl.2da instead of overriding](https://github.com/Gibberlings3/SpellRevisions/pull/116): as the name says; instead of overwriting `hidespl.2da` tables, patch them. Subsequently refined in [Fix hidespl.2da patching in tobex](https://github.com/Gibberlings3/SpellRevisions/pull/126).
27. [Imprisonment vs. Freedom patches](https://github.com/Gibberlings3/SpellRevisions/pull/118):
28. [Patch inquisitor true seeing](https://github.com/Gibberlings3/SpellRevisions/pull/119):
29. [Wrong dice in Talos' Lightning Bolt](https://github.com/Gibberlings3/SpellRevisions/pull/124): a sleuth of fixes to the Cleric of Talos' version of Lightning Bolt (more than the title suggests).
30. [rc5 fixes](https://github.com/Gibberlings3/SpellRevisions/pull/132): patch by subtledoctor to fix issues with 232 opcodes in Sleep, Magic Fang, etc.
31. [Find Traps fix](https://github.com/Gibberlings3/SpellRevisions/pull/138): Fix a targeting bug in the cleric Find Traps spell.
32. [Saves Component](https://github.com/Gibberlings3/SpellRevisions/pull/139): the code copying the new, revised saving throw tables has been relegated to its own component.
33. [Work around crashes with opcode 324](https://github.com/Gibberlings3/SpellRevisions/pull/148): Change `kreso_eestatsr.tph` opcode 324 -> 318 in spin561, spin642 and spwi022 to work around crashes.

## Earlier versions.

For earlier versions, see [Previous Changelog](./change-log.txt).
