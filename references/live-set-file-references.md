# Live Set File References

Open when you need guidance on Live Set File References in Ableton Live.

Context: [Live Sets](managing-files-and-sets.md#54-live-sets).

<a id="source-546-viewing-and-changing-a-live-sets-file-references"></a>
### 5.4.6 Viewing and Changing a Live Set’s File References

The current Live Set’s referenced files can be listed by picking the Manage Files command in the File menu, pressing the Manage Set button, and finally pressing the View Files button. A single row then appears for every file the Live Set draws upon. Expanding a row with its triangle reveals each clip or instrument within the Live Set that genuinely relies on that file. Your available actions are these:

- Replace a file — Grab a file in the browser and drop it onto a row in the listing, and the Live Set will point to the replacement rather than to the previous file. With samples that feed audio clips, the clip properties stay intact; whether the Warp Markers survive depends on length — they persist when the substitute sample matches or exceeds the original’s duration, and are dropped if it falls short. Be aware that swapping a sample affects every clip across your Set that points to it.
  In the File Reference List, Files Can Be Dropped Onto Each Entry.
- Hot-swap files — The Hot-Swap button sitting at the left edge of each row lets you flip rapidly through other candidates for whatever file is referenced at that moment. Think of it as a faster equivalent to dragging files onto the row.
  The File Reference List’s Hot-Swap Button.
- Edit a referenced sample — done through an outside program (selectable under the Settings’ File/Folder tab). Pressing the Edit button hands the referenced sample off to that outside program for editing. For as long as the Edit switch stays active, the sample is held offline. When the sample belongs to an audio clip, its existing Warp Markers survive only when the sample’s length is unchanged. Keep in mind that the Edit button applies solely to samples and not to anything else, like [Max for Live devices](https://www.ableton.com/en/live-manual/12/max-for-live/#max-for-live).
  The File Reference List’s Edit Switch.
- View a file’s location — The Location column reports whether a [file is missing](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#locating-missing-files), or whether it sits in your User Library, inside a Project, or somewhere else (“external“). Expanding the row reveals exactly where in the Set that file gets used.
  The File Reference List’s Location Column.
