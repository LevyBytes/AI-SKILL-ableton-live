# Project Sets Presets And File Management

Open when you need guidance on Project Sets Presets And File Management in Ableton Live.

Context: [Live Projects](project-files-repair-and-collection-routes.md#55-live-projects).

<a id="source-551-projects-and-live-sets"></a>
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

<a id="source-552-projects-and-presets"></a>
### 5.5.2 Projects and Presets

Fresh instrument and effect presets land in your active Project by default. Sometimes, though, putting a preset elsewhere — another folder, or your User Library — makes better sense, since that opens it up to your other Projects. Once you’ve [saving it](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#saving-presets) you can drag a preset from one folder to another; alternatively, drag the device’s title bar across a folder in the sidebar, hold until its content pane opens, and drop it into that content pane to file it there.

Should the presets you’re saving include samples and head for a fresh spot, whether Live duplicates the samples hinges on how the Collect Files on Export chooser is set in the Library Settings. You then enter a fresh name for the device, or accept Live’s proposal by pressing Enter.

<a id="source-553-managing-files-in-a-project"></a>
### 5.5.3 Managing Files in a Project

A handful of handy tools for handling Projects come with Live’s File Manager. After opening a Live Set belonging to whichever Project you mean to manage, pick the Manage Files command from the File menu and press the Manage Project button. The File Manager then gives you a rundown of what the Project holds, together with tools to:

- Locating files that the Project is missing.
- [Collecting external files](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#collecting-external-files) into the Project folder.
- Listing [unused files](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#finding-unused-files) in the Project.
- [Packing a Project](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#packing-projects-into-packs) in Pack format.
