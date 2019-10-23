# warcraft3-hotkey-editor

A [hotkey editor for *Warcraft III*](https://jcfields.gitlab.io/warcraft3-hotkey-editor/) written in JavaScript. Includes all units and structures from standard multiplayer and the official campaigns. In addition to editing hotkeys, it also allows editing tooltip text with a simplified syntax and repositioning buttons by drag-and-drop.

## Limitations

There are a few known limitations of the editor:

- The default hotkey settings are for *The Frozen Throne* multiplayer. There are a handful of differences with *Reign of Chaos* multiplayer and both campaigns that the editor does not properly reflect. For example, in *Reign of Chaos*, the Far Seer and Beastiary have their commands in a different order and several units have different names.
- The editor cannot edit button positions for the "learn hero ability" submenu (i.e., the "Researchbuttonpos" attribute). It is also technically possible for there to be a conflict between a "learn" hotkey (i.e., "Researchhotkey") and the cancel button, which the editor will not be able to detect (though this is highly unlikely since most users will leave the cancel button mapped to the escape key).
- The icon order algorithm may not be exactly the same as the game in cases where there are button position conflicts (which, by default, includes several creeps).
- There are some special creeps and other units in the campaign that can potentially be player-controlled (through mind control abilities or otherwise) that may not be available in the editor, though their commands are typically present in the standard multiplayer creeps.

## Acknowledgments

Used [RivSoft's Warcraft III data viewer](https://wc3.rivsoft.net/) for data and assets and [WTii's unit tester map](https://www.hiveworkshop.com/threads/wtiis-unit-tester.239333/) for testing.

## Authors

- J.C. Fields <jcfields+gitlab@gmail.com>
- Includes [QWEASZ hotkey set](https://www.reddit.com/r/WC3/comments/69p3nv/improved_custom_hotkeys_setup_by_wtvr/) by WTVR

## License

- [MIT license](http://opensource.org/licenses/mit-license.php)

## See also

- [*Starcraft II* Hotkey Editor](https://gitlab.com/jcfields/starcraft2-hotkey-editor)—A similar editor derived from this project.
