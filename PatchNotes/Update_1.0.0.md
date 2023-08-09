Minimize and Restore inspector window functionality. This update brought to you by Robb#6731




This update adds the ability to minimize an inspector window
(opened with the chat command `/inspect`)
again at a later time by using the `/inspect` chat command again.
Should save a lot of time re-navigating to assets.

To minimize a window, simply press the minimize button instead of the close button in the title bar.
Minimized windows preserve everything you had open previously.
Behind the scenes, it just hides the widget and returns focus, as opposed to removing it from viewport.

This feature does not affect the inspector widget built into the mod configuration screen.
