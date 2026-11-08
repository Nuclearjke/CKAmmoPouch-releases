# CK Ammo Pouch

A **WoW Forever** addon for hunters: know how much ammo you have, and where to buy more before you leave town.

**Status: test version.** Please report problems; a BugSack error text helps most.

## Install

**With WowUp:** Get Addons → *Install from URL* → paste `https://github.com/Nuclearjke/CKAmmoPouch-releases`.
WowUp will then keep it up to date from this page's releases.

**By hand:** download `CKAmmoPouch-<version>-forever.zip` from [Releases](../../releases) and extract it into
`World of Warcraft\_forever_\Interface\AddOns\`, so that you get `AddOns\CKAmmoPouch\CKAmmoPouch.toc`.
Then `/reload`.

The addon only runs on hunters.

## What it does

- **Ammo counter.** An icon with your ammo count. It turns yellow under 1000 and red under 400; you can change both.
- **Leave-town reminder.** Each time you leave a resting area, it shows your ammo and names the nearest vendor in
  chat, with a link that pins them on your map.
- **Nearest ammo vendor.** It looks in your zone first, then on your continent, and suggests the best ammo for your
  weapon and level. Vendors you open are remembered.
- **Vendor triangle.** A green triangle floats over NPCs that sell your ammo type. It's drawn on their friendly
  nameplate, so **the addon turns friendly NPC nameplates on once**. You can turn the triangle off in settings.
- **Mongoose Bite pop-up.** A large icon when Mongoose Bite is ready to use.
- **Aspect alert.** A warning when you enter combat with Cheetah, Pack or no aspect on.

## Settings

Left-click the minimap icon, or type `/ammo options`. Right-click the minimap icon for your ammo and nearest vendor
in chat. `/ammo help` lists the other commands.

## Known gaps

- It's still being tested in game. The vendor triangle and the aspect alert's latest fixes haven't been confirmed yet.
- If the aspect alert fires while you do have an aspect on, please send the `aspect buffs:` line from `/ammo debug`,
  run out of combat with the aspect on.

## Credits and license

- MIT (see `LICENSE`).
- Item and map data: World of Warcraft client tables via wago.tools.
- Ammo vendor positions: Wowhead.
- Bundled libraries: LibStub, CallbackHandler-1.0, LibDataBroker-1.1, LibDBIcon-1.0, under their authors' terms.
- World of Warcraft names and data © Blizzard Entertainment.
