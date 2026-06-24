# Managing Files And Sets (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Multiple Template Sets in the User Library.

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

### 5.5 Live Projects

A _Live Project_ is a directory holding the related Live files that go together. Picture working on a track, for instance: you begin from a blank Live Set; recording audio generates fresh sample files; you pull samples in from your collections; and as you go you store several versions of the Live Set so later comparison and rollback stay possible. You might additionally store Live Clips or device presets tied to that specific composition. Everything connected to that track is kept by this Live Project’s folder — and the tools to manage it all come from Live’s [_File Manager_](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#managing-files-in-a-project).

### 5.5.1 Projects and Live Sets

Saving a Live Set with a fresh name, or to a different directory, prompts Live to make a new project folder and place the Live Set inside it — the exception being when your save target is an already-existing Live Project. An example will make the workflow clear:

Suppose we’ve captured some audio in a brand-new Live Set. We then save that Live Set as “Tango“ onto the Desktop. The Desktop shows up in the browser since we added it earlier as a user folder. The Live browser shows this outcome:

A Live Set and its Recordings in a Live Project Folder.

Inside the project folder (“Tango Project“) sit the Live Set (“Tango.als“) plus a Samples folder, and within that lives a Recorded folder holding a pair of samples. Observe, too, that the title bar of Live’s application window names the active Project.

Now we capture an additional track into our Project. To avoid losing the earlier one, we save this changed Live Set under a fresh name. Going with the Save As command’s suggested default, the song’s newest version lands in the Tango Project folder.

The Project Now Holds a Second Live Set Version.

At this point the Tango Project holds two Live Sets, and the samples relied on by both sit together in its Samples/Recorded folder.

Time for a change of pace: via the File menu’s New Live Set command we lay down a samba number. Since it bears no relation to our tango efforts, we opt to store it somewhere other than the Tango Project folder — the Desktop, say. A fresh project folder called Samba Project then appears beside Tango Project.

A New Project Was Added Next to Tango Project.

Up to here we’ve covered making Live Projects and tucking Live Set versions into them. But what’s the way to open a Project? You just open whichever Live Set it holds. A double-click on “Tango with Piano.als“ launches both that Set and its Project — which Live’s title bar then shows.

Imagine that while working on “Tango with Piano.als“ we drift off course: the music turns into something quite different, and it strikes us that it deserves a Project all of its own. We therefore do a “Save As…“ with a new name, into a spot beyond the present Project — the Desktop, for example:

Storing a Live Set Beyond its Original Project Spawned a New Project.

Observe that the freshly made project folder doesn’t yet hold a Samples folder. “Electro with Piano.als“ continues to point at the piano sample over in the original Tango Project. That arrangement is fine in itself — the catch arrives only if the Tango Project gets relocated or removed, at which point “Electro with Piano.als“ ends up with samples missing. To guard against that, use [collecting external files](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#collecting-external-files). And even later on, Live’s search facilities for [missing files](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#locating-missing-files) can address the issue.

In truth there’s no requirement that a Project’s Live Set sit precisely one tier beneath the Project. You’re free to add as many sub-folders inside a project folder as you wish and shuffle files about to arrange them however suits you, though afterward the File Manager may be needed to “teach“ the Project about the [changes you’ve made](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#how-can-i-save-presets-into-my-current-project).

Broadly speaking, Live will go as far as it can toward heading off scenarios like orphaned (Project-less) Live Sets, since those can muddle both you and Live’s own file-management machinery. What it can’t govern, though, are cases where Sets or files get shuffled around out of sequence and thrown into disarray through the Explorer (Windows)/Finder (Mac).

_A note for users of older Live versions_: To sidestep compatibility trouble, Live refuses to overwrite Live Sets authored by earlier major versions. You’ll be prompted to “Save As…“ instead. Following that path guarantees the freshly stored Live Sets end up inside project folders.

### 5.5.2 Projects and Presets

Fresh instrument and effect presets land in your active Project by default. Sometimes, though, putting a preset elsewhere — another folder, or your User Library — makes better sense, since that opens it up to your other Projects. Once you’ve [saving it](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#saving-presets) you can drag a preset from one folder to another; alternatively, drag the device’s title bar across a folder in the sidebar, hold until its content pane opens, and drop it into that content pane to file it there.

Should the presets you’re saving include samples and head for a fresh spot, whether Live duplicates the samples hinges on how the Collect Files on Export chooser is set in the Library Settings. You then enter a fresh name for the device, or accept Live’s proposal by pressing Enter.

### 5.5.3 Managing Files in a Project

A handful of handy tools for handling Projects come with Live’s File Manager. After opening a Live Set belonging to whichever Project you mean to manage, pick the Manage Files command from the File menu and press the Manage Project button. The File Manager then gives you a rundown of what the Project holds, together with tools to:

- Locating files that the Project is missing.
- [Collecting external files](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#collecting-external-files) into the Project folder.
- Listing [unused files](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#finding-unused-files) in the Project.
- [Packing a Project](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#packing-projects-into-packs) in Pack format.

### 5.6 Locating Missing Files

Should you open a Live Set, Live Clip or preset whose referenced files are absent from where they’re supposed to be, a warning appears in Live’s Status Bar (which sits along the bottom of the main screen). Any clips and instrument sample slots tied to absent samples show up flagged “Offline,“ and rather than the missing samples Live outputs silence.

Tools to mend these broken links come with Live’s File Manager. Reach them by clicking the Status Bar message. (That’s really just a quick route to picking the Manage Files command from the File menu, pressing Manage Set, and then pressing the Locate button over in the Missing Files section.) What the File Manager then shows you is the roster of absent files alongside their controls.

The File Manager’s List of Missing Files.

### 5.6.1 Manual Repair

Repairing a broken file reference by hand means finding the absent file in the browser, dragging it across to the File Manager, and releasing it on its matching row within the missing-files roster. Bear in mind that Live makes no check of whether the file you supply truly is the one that went missing.

### 5.6.2 Automatic Repair

For mending file references, Live includes a handy automatic search routine. Kick off a search by pressing the Go button in the Automatic Search section. The neighboring triangular-shaped button unfolds finer controls for steering how that automatic search behaves.

Automatic Repair Options in the File Manager.

- _Search Folder_ — brings a folder of your choosing, plus all of its sub-folders, into the search. Pick that folder by pressing the matching Set Folder button.
- _Search Project_ — brings this Set’s project folder into the search.
- _Search Library_ — brings the Live Library into the search.

The automatic search routine might turn up any quantity of matches for each absent file. The various outcomes to weigh are:

- _No candidate found_ — pick a different folder and have another go, or track the sample down by hand.
- _One candidate found_ — Live takes the match and treats the matter as resolved.
- _Several candidates found_ — Live needs you to help out: press the Hot-Swap button (that’s the very first item on each row of the missing-files roster) so the browser shows the matches in Hot-Swap Mode. From there you can double-click the matches in the browser to load them, with playback running if that suits you.

### 5.7 Collecting External Files

So that a Live Set won’t end up with broken file references, Live lets you collect (that is, copy) them into the Set’s project folder. The File Manager is how you do it:

- Choose the Manage Files command from the File menu
- Click the Manage Set button
- Unfold the triangular-shaped fold button in the External Files section.
  Options for Collecting External Files.

Broken out by where they live (other Projects, the User Library, ones placed there by factory Packs, and the rest — sample libraries off external drives, for instance), the File Manager offers up:

- A file count and the associated disk space used;
- A Show button that will list the files in the browser;
- A Yes/No toggle for engaging or disengaging collection.

Note: Be sure to lock in what you’ve chosen by pressing the File Manager’s Collect and Save button!

The File Manager’s Collect and Save Button.

A quick route is the File menu’s Collect All and Save command, which gathers and stores every external file the current Set draws on, those out of Live’s Core Library or other installed Packs included. Watch out, since this may trigger heavy copying — particularly when your Live Set leans on big multisample libraries!

### 5.7.1 Collect Files on Export

Dragging Live Clips, device presets or tracks into the Browser to save them hands the copying of their related files over to Live, which acts on whatever you’ve picked in the Collect Files on Export chooser within the Library Settings. The choices on offer in that chooser are:

- _Always_, which is the default, silently duplicates files into whatever folder holds the clip, preset, or track.
- _When Ask is selected_, a dialog pops up from Live presenting your file-copying choices.
- _Never_ means that files will not be copied when saving.

### 5.8 Aggregated Locating and Collecting

Rather than tackling these snags mid-flow while you’re feeling creative, you might rather set aside a block of dedicated housekeeping time and clear them all at once. With Live’s File Manager you can hunt down missing files and gather external ones not just for the current Live Set, but equally for:

- _The User Library_ — pick the Manage Files command in the File menu, after which you press the Manage User Library button.
- _The current Live Project_ — pick the Manage Files command in the File menu, after which you press the Manage Project button.
- _Any Live Project_ — within the browser’s content pane, right-click a Project and pick the Manage Project option.
- _Any selection of Live Sets, Live Clips, Live Presets_ — right-click whichever items apply in the browser, then pick the Manage Files command.

Don’t forget to press the Collect and Save button down at the foot of the File Manager once you’ve wrapped up. If you skip it, what you changed gets thrown away.

### 5.9 Finding Unused Files

The unused files within a Project can be tracked down for you by Live’s File Manager. After that you’re free to look them over and choose to remove them one at a time or all together. While hunting for “unused“ files, Live examines every file inside a Project folder and tests whether any of that Project’s Live Sets, Live Clips or device presets refer to it. Should nothing do so, the file counts as unused — _even if other Projects or programs still use it_.

To turn up the unused files for whichever Project is open at the moment, pick the Manage Files command from the File menu, press the Manage Project button, and then press the triangular-shaped fold button beside “Unused Files“ to reach a summary plus the Show button. Pressing that Show button has the browser display the unused files; from there you’re able to [preview samples](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#previewing-files) and remove any you wish.

You can likewise turn up the unused files by way of the Library: pick the Manage Files command from the File menu, press the Manage Library button, and then look at the Unused Files section.

Finally, the unused files across all Projects under a given folder (and its sub-folders) can be found too: right-click a folder in the browser, choose the Manage Projects command, and consult the Unused Files section. Live examines each Project on its own and tags a file as unused even when another Projects sitting in that same folder happens to use it. _Guarding against loss, it’s wise to gather the files into the Projects they belong to before clearing out each Project’s unused files_.

### 5.10 Packing Projects into Packs

For tidy archiving and sharing, Live’s File Manager lets you pack a Live Project into Pack format. The route is to pick the Manage Files command from the File menu, press the Manage Project button, and then press the triangular-shaped fold button beside “Packing.“ Pressing the Create Pack button opens a file-select dialog for naming and placing a fresh Pack file. Building a new Pack out of a Project leaves that Project untouched. Should you want rid of the Project, you can delete it through the browser.

To shrink the size of Packs, Live applies lossless compression. The savings reach as much as 50 percent of the file size, depending on what audio a Project contains.

Unpacking a Pack (that is, bringing back the original Live Project) is done by double-clicking the Pack file (.alp), dragging it onto the Live main window, or finding it through the File menu’s Install Pack command.

### 5.11 File Management FAQs

### 5.11.1 How Do I Create a Project?

Saving a Live Set creates a Project on its own, _except_ in the case where you save into a Project that already exists.

### 5.11.2 How Can I Save Presets Into My Current Project?

Presets can go straight into the active project: drag from the device’s title bar and drop onto the Current Project label in the browser. After that the File Management tools are yours to use, to gather any referenced samples, and so on.

### 5.11.3 Can I Work On Multiple Versions of a Set?

When you want to develop several versions of one Live Set, store them all in a single Project. Typically that’s the Project spun up when the Live Set’s first version was saved. Holding multiple Live Sets, a Project keeps just a single copy of any samples shared among the versions, which both conserves disk space and aids organization.

### 5.11.4 Where Should I Save My Live Sets?

Live Sets may be saved wherever you please, yet because saving into folders of already-existing Projects can spawn trouble, it ought to stay an exception. Reserve saving a Live Set into an existing Project for when there’s some genuine connection to it — say, a variant version of a song the Project already holds.

### 5.11.5 Can I Use My Own Folder Structure Within a Project Folder?

Files inside a Project may be arranged however you like, but the File Manager is needed to re-link whichever files you shifted about:

1. Whether through Live’s Browser or from your operating system, rearrange the folders and files that sit inside your Project folder.
2. Head to the Project folder within the Browser, then pick Manage Project from its context menu.
3. Where you’ve relocated any of the Project’s samples from where they were, that gets flagged in the File Manager’s Missing Samples section. Press the Locate button to go looking for those samples.
4. Because all your samples are known to live in the Project folder, open up Automatic Search. Next, switch on both the Search Project and Fully Rescan Folders options. To launch the hunt, press Go at the end.
5. Once the search wraps up, refresh the Project by pressing Collect and Save down at the foot of the File Manager.
   </content>
   </invoke>
