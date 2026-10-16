# Live Set Saving Merging And Templates

Open when you need guidance on Live Set Saving Merging And Templates in Ableton Live.

Context: [Live Sets](managing-files-and-sets.md#54-live-sets).

<a id="source-541-creating-opening-and-saving-sets"></a>
### 5.4.1 Creating, Opening and Saving Sets

Fresh Live Sets come from the File menu’s New Live Set command, while the Open Live Set or Open Recent Set command brings up existing ones. From the browser, a double-click on a Live Set, or pressing Enter on it, opens it as well.

The File menu’s Save Live Set command stores the current Live Set precisely as it stands, clips and settings and all.

To save the current Live Set under another name and/or in another directory location, reach for the Save Live Set As command; the Save a Copy command instead spawns a duplicate of the current Live Set bearing a new name and/or new directory location.

<a id="source-542-accessing-a-sets-undo-history"></a>
### 5.4.2 Accessing a Set’s Undo History

Every action carried out since a Set was opened shows up in the Undo History, which can roll them back or restore them up to any chosen point. Reversing or recovering a whole batch of actions in one move is therefore simple, with no need to undo or redo each step on its own.

Bring up the Undo History by picking the _Undo History_ entry from the View menu, or with the shortcut Ctrl+Alt+Z (Win) / Cmd+Option+Z (Mac).

The Undo History for a Set.

After it opens, the actions appear in the sequence they happened, newest sitting at the top and oldest at the bottom. To roll the Set back to a given action in its history, pick that action by clicking it or by stepping to it with the up and down arrow keys and hitting Enter. Whatever actions sit above the one you chose turn grey, signalling that they've been undone, while the actions beneath it stay live since their changes are still in force. Choosing a greyed-out action reinstates it together with any other undone actions sitting below it.

Be aware that closing a Set discards its Undo History rather than storing it, and the list resets whenever the Set is opened again. Live regards creating or opening a Set as the opening entry in the Undo History, which is why that step can't be undone.

<a id="source-543-merging-sets"></a>
### 5.4.3 Merging Sets

Merging Sets is painless in Live, which proves useful for pulling together work from separate versions or pieces. To bring every track (the return tracks aside) of one Live Set into another, drag the Set out of the browser into the current Set and drop it on any track title bar or onto the drop area beside or beneath the tracks. The tracks from the dropped Set are rebuilt in full — their Session and Arrangement View clips, their devices, and their automation all carry over.

The Session View zone where Live Sets are dropped to import them.The Arrangement View zone for dropping Live Sets to import them.

When you'd rather grab single tracks out of a Set, the Live Set can be unfolded inside the browser exactly as though it were a folder.

Unfolding a Set to Reveal its Contents.

At this point you can drag those individual tracks and drop them following the method laid out at the start of this section. Whatever [grooves](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves) were saved alongside your Set also turn up as a folder inside the unfolded Set.

Should you be after only the device chain — say a device plus its audio or MIDI effects — from another Set, drag the Devices icon out of that Set in the browser.

The Devices Icon in an Expanded Live Set.

Dragging [Group Tracks](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks) and nested Group Tracks straight from Live’s browser works too. Group Tracks open up in the browser, which lets you pull a single track out from inside.

Beyond unfolding Sets themselves, you can open up the tracks within them to reach the individual Session View clips that were placed on the track:

Revealing the Session View Clips Contained in a Set.

Session View clips from the Set can be browsed, previewed and imported just as if each had been kept as its own Live Clip. The upshot is that any Live Set may act as a sound pool for any other, inviting creative reuse and crossover.

<a id="source-544-exporting-session-clips-as-new-sets"></a>
### 5.4.4 Exporting Session Clips as New Sets

A group of Session View clips can become a brand-new Live Set when you drag them onto the browser. Begin by selecting several Session View clips at once — click and drag, or hold the Shift or Ctrl (Win) / Option (Mac) modifiers. With your selection made, drop those clips onto the Current Project or some user folder; there you'll either accept the name Live proposes or supply your own.

<a id="source-545-template-sets"></a>
### 5.4.5 Template Sets

Reach for the File menu’s Save Live Set As Default Set… command to store the current Live Set as your default template. From then on Live treats those settings as the starting, default state every new Live Set inherits. This lets you set up in advance:

- The way your multichannel input/output is arranged.
- Ready-made devices such as EQs and Compressors sitting in each track.
- [Computer key mappings](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control).
- [MIDI mappings](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-remote-control).

Keep in mind that any template Set shown in Live’s browser may be promoted to the default Live Set through the Set Default Live Set entry, found in the Set’s context menu or the File menu.

Beyond that single default template, you're free to build extra template Sets aimed at different kinds of projects, each carrying its own distinct layout of tracks, devices, and the like. The way to do this is to save the current Live Set with the File menu’s Save Live Set As Template… command. Whatever you save this way shows up in the browser’s Templates category and in the User Library's Templates folder. That Templates folder under the User Library springs into existence on its own the first time a template Set is saved. These Sets behave as templates from then on: they open with the configuration you stored but carry the name Untitled.als, primed to serve as a new Set.

<a id="source-managing-files-and-sets-part-2"></a>

Multiple Template Sets in the User Library.
