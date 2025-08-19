# Content Inspector

#### This mod is a tool intended to assist mod developers, and has limited usefulness for typical players.

For a brief walkthrough of using this tool, see the [ContentInspector Tutorial on the ContentLib documentation](https://docs.ficsit.app/contentlib/latest/Tutorials/ContentInspector.html).

For support, join the [Nog's Mods discord server](https://discord.gg/kcRmFxn89d).

**ContentInspector** is an in-game debugging tool created by Nog that allows you to **view**, temporarily **modify**\*, and **export to JSON** the following:

- Mod and base-game content
- Script-generated content (such as that loaded by [ContentLib](https://ficsit.app/mod/ContentLib))
- Property values on every loaded Actor in the game world
- Probably more I (Robb) am not aware of

\**(Note: success with modification of properties may vary)*

This is useful for:

- Discovering the location of game assets
- Finding out what properties an actor has at runtime that can't be determined from the editor
  - Finding out the value of blueprint-defined variables at runtime
  - Finding out what Socket an attachment actor is attached to)
- Comparing exports of actors taken at different times to find out what changed between
- Checking what mod content actually ends up registered
- Whatever you want to use it for!

To open the inspector in-game, you can use the chat command `/inspect`,
or the widget built into the Mod Configs screen (useful on the Main Menu).

To inspect a specific in-world actor, stand near it and look at it,
then use the `/inspect this` chat command.
The widget's title bar will show information about what the trace found.

If you want to return to a window later in your game session,
you can use the minimize button.
The same window will be restored when you use `/inspect` again.

It is quite possible to crash your game session by modifying various properties.
Do not expect to receive support for crashes caused by changes you make with this tool.
Any modifications will not persist between game sessions.

It is possible to dump and generate Blueprints or some Assets (Curves, Material stubs, etc.) with ContentInspector,
but it's highly advised to use the
[Asset Toolkit](https://docs.ficsit.app/satisfactory-modding/latest/CommunityResources/AssetToolkit.html)
instead, since asset generation is not the purpose of this mod.

Depends on [JsonStructs](https://ficsit.app/mod/JsonStructs), a hidden mod.
Will be installed automatically when you install this mod via SMM.
Note that fields prefixed with `JS_` are created by JsonStructs and contain metadata about the field being inspected.

Inspecting the Fuel Generator in Widget view mode:

![Widget inspect](https://i.imgur.com/yEI6xB2.jpg)

Viewing loaded ContentLib script content:

![Script Content](https://i.imgur.com/y7lEIhg.png)

Inspecting a ContentLib script asset (from the RePan mod) in Text view mode:

![Text Inspect](https://i.imgur.com/KjsvkDz.png)
