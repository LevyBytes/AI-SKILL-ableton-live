# VST Folders Presets And Banks

Open when you need guidance on VST Folders Presets And Banks in Ableton Live.

Context: [VST Plug-Ins](device-presets-and-plug-in-routes.md#234-vst-plug-ins).

<a id="source-2341-the-vst-plug-in-folder"></a>
### 23.4.1 The VST Plug-In Folder

On your initial Live launch, your VST plug-in sources have to be activated before you can work with VST plug-ins. Your platform may also require you to point Live at the VST plug-in folder that holds the devices you intend to use. To configure your VST sources, click the Activate button within the browser's Plug-Ins panel, or bring up the Plug-Ins Settings via Ctrl+, (Win) / Cmd+, (Mac). The Plug-In Sources section is located there.

The VST Plug-In Sources for Windows.

On Windows, do the following:

1. Point Live at your VST plug-ins through the VST Plug-In Custom Folder entry: click the _Browse_ button, which opens a folder-search dialog where you locate and choose the right folder.
2. After you've chosen a VST Custom Folder and Live finishes scanning it, the path appears. On Windows, keep in mind that Live might have located a path in the registry, sparing you the browsing step.
3. Confirm that the Use VST Plug-In Custom Folder option reads “On,“ which keeps your chosen folder an active VST plug-in source in Live. If you'd rather not use your VST plug-ins in Live, switch the Use VST Plug-In Custom Folder option off.
   The VST Plug-In Sources for macOS.

To configure your VST plug-ins on macOS, do this:

1. Typically your VST plug-ins land in this folder within your home and local directories: /Library/Audio/Plug-Ins/VST. The Use VST plug-ins in System Folders option toggles Live's use of them on or off.
2. You might keep a separate folder for your VST plug-ins (say, the ones reserved for Live). VST plug-ins in that folder can be used alongside the System folder ones or in their place. To point Live at this folder, click the Browse button beside the VST Plug-In Custom Folder entry, opening a folder-search dialog where you locate and choose the right folder.
3. Keep in mind that the Use VST Plug-In Custom folder option lets you switch off the VST plug-ins in this folder.

After your Plug-Ins Settings are configured, the browser shows every plug-in it locates within the chosen VST plug-in folder(s) plus any sub-folders.

You can likewise use VST plug-ins kept in other folders on your machine. To do that, make a macOS or Windows _alias_ of the folder containing the extra VST plug-ins, then drop that alias into the VST Plug-In Custom folder (or, on macOS, the VST Plug-In System folder) chosen in Live's Plug-Ins Settings. An alias may reference a separate partition or drive on your computer. Live scans the designated VST plug-in folder along with any alias folders inside it.

A handful of VST plug-ins are flawed or simply don't work with Live, and during scanning they can crash the program. On your next Live launch, a dialog tells you which plug-in triggered the trouble. Based on what Live determines about it, you may be offered a choice between running another scan or disabling the troublesome plug-in. Pick rescan and have them crash the program again, and Live disables them on its own; they then stay out of the browser and won't be rescanned until you reinstall them.

<a id="source-2342-vst-presets-and-banks"></a>
### 23.4.2 VST Presets and Banks

Each VST plug-in instance “owns“ a _bank of presets_. The intent of a preset is to hold a single full set of values for the plug-in's controls.

Pick a preset out of the plug-in's bank using the chooser beneath the title bar. Each bank holds a fixed count of presets. At any moment you operate “in“ the preset currently chosen, meaning every edit you make to the plug-in's controls folds into that selected preset.

The VST Plug-In Preset Chooser.

Keep in mind that VST presets aren't the same as Live device presets: a Live device's presets are common to all of its instances and Live Sets, whereas VST presets “belong“ to that one particular instance of the VST plug-in.

Rename the active preset by selecting the VST's Device Title Bar and running the Rename Plug-In Preset command from the Edit menu. Then enter a fresh preset name and press Enter to confirm.

Renaming a VST Plug-In Preset.

You can load VST presets and banks in from files. A VST's Load Preset or Bank button opens a standard file-open dialog where you track down the file you want.

On the Left, the VST Load Preset or Bank Button; on the Right, the Save Preset or Bank Button.

_Windows only_: In the Windows dialog, use the File Type filter to indicate whether you're after VST Presets (VST Program Files) or VST Banks (VST Bank Files).

To write the chosen preset out to a file, click the VST Save Preset or Bank button for a standard file-save dialog; in the Format menu (Mac), or alternatively the File Type menu (Windows), pick “VST Preset,“ then choose a folder and a name. Writing out the whole bank as a file works the same way, except you select “VST Bank“ as the file type/format.
