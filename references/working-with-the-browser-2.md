# Working With The Browser (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Most Packs ship with a Pack Info page that lists who built the Pack, a brief description of what it contains, and occasionally a walkthrough to get you started. To see the Pack Info pages for every Pack you have installed, choose the Pack Overview option under the Help menu; alternatively, reach a single Pack's info page straight from the browser by choosing Show Pack Info in the context menu of any installed Pack.

Open a Pack Info Page from the Browser.

Keep in mind that no Pack Info page is provided for the Core Library.

### 4.7.3 Splice

Splice offers a royalty-free collection of samples you can dig through to find fresh sounds and lift the quality of your productions. Because Live ties in with Splice directly, you can reach that collection right from the Splice label in the browser.

The Splice Label.

Clicking the Splice label brings up the Home page. There you'll find four sample category buttons for starting your exploration of the Splice library, plus the search bar, the navigation bar, and a Search with Sound drop area. The arrows in the navigation bar let you move back and forth through every action you've performed inside the Splice label.

Near the top of the label's content pane you'll also see the controls for signing in or registering a free Splice account.

By default the Splice label sits in the sidebar, though you can remove it either by right-clicking the label and choosing “Hide from Sidebar”, or by switching the “Show Splice” option in Live’s Library Settings to Off.

The Show Splice Option in Live’s Settings.

Bear in mind that a live internet connection is needed before any content shows up in the Splice label.

#### 4.7.3.1 Logging Into Splice

Browsing and previewing samples works right away when you open the label, but signing in with your Splice account is required before you can drop samples into a Set, keep samples in your Splice library, or run the Search with Sound feature. To sign in, hit _Login_ near the top of the content pane; if you haven't set up a Splice account yet, use the _Try free_ button instead. Either choice launches your operating system's default web browser and sends you to Splice’s website, which then shows a device confirmation code. That identical device confirmation code appears at the same moment in the Splice label inside Live. Confirm that both codes match, then click _Confirm_ in the web browser.

The Device Confirmation Code Displayed in the Splice Label.

After the device is confirmed, your web browser opens a login page where you can either supply your current Splice account credentials or register a brand-new account.

Splice’s Login Page.

After you've signed in to your Splice account, the label's Home page changes a little: the Library icon in the navigation bar is no longer dimmed and now opens your collection of Splice sounds, the sample category buttons give way to a different set of browsing buttons relocated to the top of the page, and the Search with Sound drop area shifts down to the bottom of the page.

The Splice Label UI When Logged In.

#### 4.7.3.2 Searching for Splice Samples

Hunting for samples can be done straight through the search bar. Selecting it brings up the popular search categories, and from there you can either pick one of those suggestions or begin typing whatever term you have in mind. As you type, additional suggestions appear.

The Suggestions Displayed After Typing In a Search Term.

Pick one of the suggestions, or hit Enter, to show the results. After that, switch between the “Samples” or “Packs” option at the top of the results to see either individual samples or sample packs matching your search term.

A List of Individual Samples in the Search Results.

The filters and tags sitting above the results let you narrow things down further. Available filter dimensions include key, tempo, music genre, instrument type, and whether the sample type is one-shot or loop. Which tags appear beneath the filters depends on the search term and sample category at hand; clicking the three dots button on the right end of the list reveals the full tag list.

For ordering, the results can be arranged by most popular, relevant, or recent samples, and you can also scramble the list by choosing the “Random” option from the drop-down menu or hitting the shuffle button.

Be aware that with a free Splice account (or when you aren't signed in), only the samples bundled with that account show up in the results; this is flagged by the _Included_ filter above the search results and the “included” tag shown beside individual samples. A free Splice account ships with roughly 2,500 samples.

Search Results Displayed for a Free Account.

Beyond the search bar, the browsing buttons on the Home page give you another way to look for samples. Three buttons are available: Instruments, Genres, and Cinematic FX. Clicking any of them reveals a set of sample categories, and each category holds its own subcategories from which you pick one to focus your search. Within Instruments and Cinematic FX, you may also display every sample in a category without picking any subcategory at all.

Sample Categories and Subcategories.

Splice’s Search with Sound feature is yet another route, letting you track down samples that pair well with the clips you already have. Just drag a clip out of your Set onto the Search with Sound area on the Home page, or make a time selection and click within the Search with Sound area to grab the selection. Splice processes the audio and hands back a list of 50 compatible samples. From the results page you can also play the sound reference again, drag in a different clip or grab a new selection, and remove the current sound reference.

Search with Sound Results.

#### 4.7.3.3 Working with Splice Samples

Typing a search term, picking a sample category, or running the Search with Sound feature each produces a list of matching samples in the content pane.

The search bar adjusts to match whatever sample category is on screen, so any term you type into it searches only the samples that fall within the category currently selected.

The Search Bar Updates When Viewing a Sample Category.

Every sample entry in the list shows a picture of the pack it comes from (clickable to open the whole pack), an icon marking the sample as a one-shot or loop, the sample name, the tags attached to the sample, and a context menu for adding the sample to Likes or Collections in your library or jumping to the sample’s pack.

Hovering over a sample swaps the sample type icon for the Play button; click that button to hear a preview of the sample. Clicking the sample name kicks off the preview on its own.

Out of the box, every sample previews on a loop, whether it's a one-shot or a loop. That behavior, along with other preview settings, can be adjusted from the options along the bottom of the content pane. As an example, loops follow your Set’s tempo by default, yet clicking the _1x BPM_ option and turning off the _Timestretch_ toggle plays a loop at its native tempo. With one-shot samples, clicking the _1 BAR_ option disables the looped preview.

Among the preview settings you'll also find a way to transpose samples to a chosen key, plus an option to follow Live’s scale settings. The preview loudness is adjustable too.

Hovering over or selecting a sample reveals a heart icon beside the sample’s name; one click on it instantly drops the sample into Likes in your library.

Widening the content pane surfaces still more sample details at once, since these columns become visible: Time, Key, and BPM.

Additional Columns Are Visible When the Content Pane is Expanded.

After spotting a sample you want, drag it onto an audio or MIDI track within your Set. In the Session View, samples can also be loaded by double-clicking them or hitting Enter. Dragging samples straight into devices like Sampler, Simpler, Drum Rack, or Impulse works as well.

Bear in mind that any clip built from a Splice sample gets its Warp Mode set to Complex automatically, no matter what default is configured in the Record, Warp & Launch Settings. That guarantees the sample plays back exactly as it did while you previewed it inside the Splice label.

Loading samples into your Set automatically [licenses](https://support.splice.com/en/articles/8652641-how-do-i-generate-a-certified-license-for-my-samples) them and stores them in your Splice library.

By default, anything you download from Splice lands in the User Library under the Splice sub-folder inside the Samples folder, but the Library Settings let you choose your own destination for Splice samples. These choices are on offer:

- User Library — saves the samples to User Library/Samples/Splice.
- Current Project — saves the samples to Current Project/Samples/Splice.
- Custom Folder — saves the samples to any location of your choosing.
  Set the Download Folder for Splice Samples.

#### 4.7.3.4 Splice Library

Inside the Library you'll find Likes and Collections, plus every sample you've previously pulled into your Sets — meaning the samples that were downloaded to whatever spot you chose in the Library Settings.

Splice Library Page.

A custom sample collection can be built either from the Collections page or via the menu within a sample entry. Clicking an existing collection lets you see the samples you've gathered in it, rename it or change its description, mark the collection private, hand out a link to it, or erase it.

#### 4.7.3.5 Splice Settings

On the Settings page you can handle your Splice subscription plan, adjust your display settings, and pull down usage logs. The page also explains how certified licenses are generated for the samples you work with, links to Splice’s knowledge base, and provides a way to send feedback to Splice.

When you aren't signed in, a Login button is shown on the page as well.

Splice Settings.

### 4.7.4 Using Ableton Cloud

With Ableton Cloud, you can keep up to eight Sets from Move and Note and reach them from any Ableton product. Once Cloud is turned on in Live, the synced Sets show up in the browser's Places section.

Turning on Cloud in Live starts with clicking the Cloud label in the browser sidebar. Doing so brings up a prompt asking you to sign in at ableton.com to grant the service access. Hit the _Sign In_ button, which opens a web browser so you can log into your ableton.com user account.

Sign In to Enable Ableton Cloud in Live.

Once Cloud is up and running, the Cloud label is where your synced Sets show up.

Synced Sets in the Browser.

Be aware that every factory and imported sample inside synced Sets lives in the [User Library](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#user-library), which has to be configured and reachable whenever you open those Sets in Live. Should you open a synced Set and notice samples are absent, verify whether your User Library points to a custom spot, like an external hard drive. Getting the samples relinked simply means ensuring that custom User Library location is plugged in and reachable.

Because syncing flows from Move or Note into Live and never back the other way, we advise running the _Collect All and Save_ command from the File menu whenever you save synced Sets you have taken further inside Live. That pulls every sample the Set relies on into one Project folder, which you're then free to store wherever you like on your machine.

Be aware that the Cloud label appears in the browser sidebar by default, but you can tuck it away by switching the “Show Cloud” option in Live’s Library Settings to Off.

The Show Cloud Option in Live’s Settings.

### 4.7.5 Transferring Files from Push 3 in Standalone Mode

Songwriting can carry on seamlessly across Push and Live: whatever Set you build in Standalone Mode on Push is openable on, or movable to, your computer. Sending Sets back over to Push to keep working when you're away from the studio is possible too, provided you stick to native devices, freeze any track that holds plug-ins, and gather all your samples into the Project folder.

Reaching Push files inside Live requires Push to be running Standalone Mode and joined to the same Wi-Fi network your computer uses. With that done, click the Push label in Places. Push then turns up in the browser’s content pane labeled with its own device name. Any other Push units nearby will appear too. When you own multiple units, look up the exact “Push xxx-xxx” name under the Status Tab of Push’s Setup menu to be sure which one you intend to pair with Live. Hit the Connect button to move forward.

Connect Push to Transfer Files.

Push then shows a six-digit code; type that code into the dialog window that pops up in Live and press OK to keep the pairing going.

When Push and Live are paired successfully, all the Project folders you saved in Standalone Mode plus Push’s User Library turn up in Live’s browser.

Push Project Folders in the Browser.

While Push stays paired with Live, you can surface any fresh Sets or edits you've made to existing Sets in Standalone Mode within Live’s browser by clicking off the Push label in Places and then back onto it to refresh the file list.

To unpair Push from your computer, right-click the Push label in Places and choose Disconnect.

Read more about continuity between Push and Live in the [Push manual](https://www.ableton.com/en/push/manual/#continuity-between-push-and-live).

Be aware that the Push label sits in the browser sidebar by default, though you can conceal it by switching the “Show Push” option in Live’s Library Settings to Off.

The Show Push Option in Live’s Settings.

### 4.7.6 User Library

Everything you save — custom presets, defaults, Live Clips, template Sets, and so on — ends up in the User Library. Since the User Library keeps its own dedicated location apart from other installed content, backing it up or moving it between separate Live installations or computers is straightforward.

When Live is first installed, the User Library is set up by default in the following place:

- Windows: `\Users\<username>\Documents\Ableton\User Library`
- Mac: `Macintosh HD/Users/<username>/Music/Ableton/User Library`

To point the User Library somewhere else, use the “Location of User Library” option found in the Library Settings.

At the start, the User Library holds almost nothing; it carries just a handful of default folders: Clips, Defaults, Grooves, Presets and Samples. You're free to introduce your own custom folders and sub-folders and to delete the default folders when you don't need them.

Folders in the User Library.

Whatever you store in your User Library also turns up under the matching Library labels.

#### 4.7.6.1 ABL Assets

Should you turn on [Ableton Cloud](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#using-ableton-cloud) and sync a few Sets across from Move or Note, the assets belonging to those Sets are kept inside the ABL Assets folder.

#### 4.7.6.2 Chord Banks

Inside the Chord Banks folder you'll find whatever custom cord banks you've saved or built to use alongside the [Stacks MIDI Tool](https://www.ableton.com/en/live-manual/12/midi-tools/#stacks).

#### 4.7.6.3 Clips Folder

The Clips folder is the home for Live Clips. To save one, just drag any clip into the folder.

Saving a MIDI clip brings along the MIDI data (notes and automation, for instance) plus whatever device settings are attached.

Saving an audio clip — or a MIDI clip running a device that points to audio samples (Drum Rack, Sampler, and the like) — also tucks the referenced samples in alongside the clip. In the Library Settings, this happens on its own provided the Browser Behavior option named “Collect Files on Export” has the value Always — and that is its default configuration.

#### 4.7.6.4 Defaults Folder

The Defaults folder is where your saved defaults live — for effects, devices, tracks, Slicing to MIDI options, and other things besides. With default presets in place, you bring back particular device settings every time that device is loaded.

For more on saving and applying default presets, look at the [Default Presets](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#default-presets) section.

To get the full picture of every default Live supports, consult the [Using Defaults](https://help.ableton.com/hc/en-us/articles/209071029) article in our Knowledge Base.

#### 4.7.6.5 Grooves Folder

Your custom groove files are kept in the Grooves folder.

A new groove can be made by pulling the timing and volume information out of any audio or MIDI clip. Do this either by dragging the clip onto the Groove Pool or by using the Extract Groove command in the clip’s context menu.

For a deeper look at how grooves function in Live, head to the [Using Grooves](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves) chapter.

#### 4.7.6.6 Presets Folder

Your saved Instrument, Max for Live, MIDI and Audio Effect presets reside in the Presets folder.

Just like when you save clips, any referenced audio samples bundled into the preset get saved too.

Within the Working with Instruments and Effects chapter, the [Saving Presets](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#saving-presets) section covers more about how device presets are stored.

#### 4.7.6.7 Samples Folder

Every referenced sample coming from saved presets, tracks, and similar sources gets stored in the Samples folder.

Depending on where those samples originate, a distinct folder for recorded or processed samples is generated the moment such samples are saved.

#### 4.7.6.8 Templates Folder

The Templates folder holds your saved template Sets along with any custom default Live Set.

For more on working with templates, see the [Template Sets](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#template-sets) section of the Managing Sets and Files chapter.

#### 4.7.6.9 Managing Files in the User Library

To get a summary of your User Library — what's in it, plus any missing or external files — pick the _Manage Files_ option from the File menu and then click the _Manage User Library_ button that shows up in the File Manager.

You Can Manage the User Library in the File Manager.

### 4.7.7 Current Project

Every file belonging to the Project you currently have loaded is held under the Current Project label.

An Expanded Live Set in the Current Project Label.

From here you can reach all the Set's tracks (with their clips and devices), the Return and Main tracks, and any grooves you've loaded.

After a Project has been saved a minimum of twice, a Backup folder shows up under the Current Project label.

Backup Sets in the Current Project Label.

That folder keeps the ten most recent saved versions of the Live Set. Backup Sets are recognizable by the timestamp shown in brackets beside the Set name. Whenever the backup count passes ten, Live removes the oldest backup Set on its own. Backups that get removed are sent to the trash bin.

This capability comes in handy when you've accidentally written over a Project file or wish to revisit an earlier version of your Live Set.

If the Live Set you're working on hasn't been saved yet, no Backup folder exists, and the current Project points to a temporary location.

Right-clicking the Current Project label and choosing Show in Explorer (Win)/Finder(Mac) opens the Project folder’s location on your computer.

For thorough detail on how Project folders and Sets behave in Live, look at the [Live Projects](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#live-projects) section of the Managing Files and Sets chapter.

### 4.7.8 User Folders

No matter where your creative tools happen to be installed on your computer, Live’s browser lets you work with them. So you might, for instance, park huge sample collections across one or several external drives and still reach their contents through the browser — there's no requirement to gather everything in one central spot.

Before you can work with your own folders in Live, they have to be added to the browser, which you do either by dragging them straight into the Places section out of the Explorer (Win)/Finder (Mac), or through the _Add Folder_ option in the browser’s sidebar.

The Add Folder Option.

Once a user folder is added, Live scans it, which “teaches” the browser what's inside. The scan's duration hinges on how many files and sub-folders the folder holds. While scanning continues, a spinning wheel sits next to the Places label. After it wraps up, the folder's files become reachable from Places.

Adding a user folder doesn't relocate the folder anywhere; it merely surfaces it within Live’s browser. Rearranging your drives through Explorer (Win)/Finder (Mac) may leave Live unable to track down user folders you've moved or renamed. On top of that, if a user folder lives on an external hard drive and Live launches while that drive is disconnected, the folder won't be located.

When Live can't locate a user folder, it still shows in the browser, only with its name dimmed. You can try tracking it down with the context menu’s _Locate Folder_ command, or have Live “forget” the folder using the _Remove from Sidebar_ command. That same command also clears out folders that aren't missing but that you've simply stopped wanting to work with.

Note: Add only specific content folders to Places instead of whole hard drives. Throwing in hard drives or extremely large folders may bog down the indexing process, or force the content to be re-indexed over and over each time Live launches.

### 4.8 Navigating in the Browser

Getting around the files in Live’s browser works with either the mouse or your computer keyboard:

- Move up and down within a browser label using the up and down arrow keys, the mousewheel, or a click-and-drag while holding the CtrlAlt (Win) / CmdOption (Mac) modifier.
- Use the left and right arrow keys to collapse and expand folders or to shift between the sidebar and content pane.

By default, opening a new folder closes whatever folders were already open, but holding Ctrl (Win) / Cmd (Mac) as you open new folders overrides that.

### 4.9 Previewing Files

Samples, clips, and instrument presets can all be previewed by Live right inside the browser. That gives you a sense of how a thing sounds before you commit a new element to your Set.

Switch on previewing by turning on the Preview toggle beside the Preview Tab at the foot of the browser.

The Preview Toggle.

With it switched on, selecting a file in the browser plays a preview. The up and down arrow keys step you through files and their audio previews.

Even with the Preview toggle switched off, you can still preview files by pressing ShiftEnter or the right arrow key while a browser item is selected.

As a file previews, the Preview Tab displays a waveform. Clicking within the scrub area jumps playback to that spot. Be aware that scrubbing isn't available for clips saved with Warp switched off.

The Preview Tab’s Scrub Area.

The Raw button starts out switched off, letting Live begin previewing files at the top of the next bar while transport is running. That helps you judge how the sound sits within your current project. Switching on the Raw button previews files at their native tempo. Audio previews loop while Raw is off and play unlooped while Raw is on.

Keep in mind that scrubbing can't be done while Raw is on.

The volume of audio previews is set with the Main track’s Preview/Cue Volume knob.

The Preview/Cue Volume Knob.
