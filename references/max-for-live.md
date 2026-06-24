# Max For Live

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 31. Max for Live

Through Max for Live, building your own devices becomes a way to broaden and personalize Live. The product offers a full set of tools for authoring instruments, effects, and MIDI Tools, and ships with a library of [built-in devices](https://www.ableton.com/en/live-manual/12/max-for-live-devices/#max-for-live-devices) plus tutorials. Within a Set, these devices behave exactly like Live’s built-in ones, and you may modify them straight from Max.

Reaching into a Live Set to read or change its components, or broadening what hardware control surfaces can do through the [Live API](https://docs.cycling74.com/userguide/m4l/live_api_overview/), is another job Max for Live handles.

Built jointly with [Cycling ’74](https://cycling74.com/), Max for Live is an add-on that opens up the Max programming environment from inside Live. For a fuller picture of everything Max enables, consult the [Max documentation](https://docs.cycling74.com/).

### 31.1 Setting Up Max for Live

Shipping inside Live Suite — and inside Standard whenever the Max for Live add-on is in use — Max for Live arrives bundled and requires no separate setup step.

Should you rather edit Max for Live devices with a particular build of the Max application instead of the one that ships bundled, point Live at the right file path under its File & Folder Settings:

Pointing Max for Live device editing at a chosen build of the Max application.

After saving the path, a Live restart is required before the change applies. From then on, the Max application you named opens whenever you [open the Max editor](https://www.ableton.com/en/live-manual/12/max-for-live/#editing-max-for-live-devices) from a Max for Live device.

### 31.2 Using Max for Live Devices

As part of Live’s Core Library, Max for Live bundles a selection of instruments and effects. The browser surfaces these under the Instruments, Audio Effects, MIDI Effects, and Modulators labels. Modulators form a dedicated category of devices whose modulation signals steer parameters across Live.

Every Max for Live device — those bundled, those arriving from installed third-party Packs, and those you have built and stored yourself — lives under the Max for Live label in the browser. Within that same label you’ll also find [Max for Live MIDI Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#using-max-for-live-midi-tools), handy for reshaping and producing notes inside MIDI clips.

A large share of Max for Live devices ship with presets of their own. These behave much like Live’s [device presets](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#live-device-presets); even so, you’re free to build new ones or adjust what exists, following the steps in the section below.

### 31.3 Editing Max for Live Devices

A Max device — frequently called a “patch” — is assembled from objects that route data between one another over virtual cables. Take the default Max Audio Effect preset: it begins from this minimal wiring, where the _plugin~_ object picks up audio arriving at the effect’s slot in the device chain and forwards it to the _plugout~_ object, which then hands the signal off to whatever devices follow downstream.

The Default Max Audio Effect Preset.

Spinning up a fresh Max device from a default means dragging a _Max Instrument_, _Max MIDI Effect_, or _Max Audio Effect_ out of the browser and into your Set. Equally, the objects inside any existing Max device preset are open to editing and tweaking.

The behavior of any given Max device comes down to which objects it holds and the way those objects are wired together. Reaching a device’s objects means opening the Max editor — also called the “patcher” — through the _Edit in Max_ entry, which sits in the context menu or in the Show Options menu of the device’s title bar.

The Edit in Max Command.

Doing so starts Max and brings the device up inside the Max editor.

The Default Max Audio Effect in the Max Editor.

In versions before Live 12.2, the device title bar carried an Edit button rather than the Edit in Max command. To bring that Edit button back, drop the -MaxForLiveDeveloperMode option into the [Options.txt file](https://help.ableton.com/hc/en-us/articles/6003224107292).

After making edits to a device, store them with either the Save or Save As command found under Max’s File menu. When a Set holds several copies of one device, Save pushes the fresh edits to every copy at once. Picking Save As instead brings up a dialog asking whether the edits should land on just the preset you edited or on all the instances.

A Max device, by default, goes into the matching User Library folder according to its device type: audio effects land in the Max Audio Effect folder, MIDI effects in the Max MIDI Effect folder, and so forth.

Sticking with the default location is advisable, since Max devices are written out on their own as AMXD files instead of being folded into a Live Set. Relocating or renaming a referenced AMXD file down the line may sever the file path it’s tied to in Live. Should that occur, the [File Manager](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#locating-missing-files) lets you track down the file and put things right.

### 31.4 Building Max for Live MIDI Tools

There are two routes to authoring your own Max for Live MIDI Tools:

1. Start from the Max MIDI Transformation or Generator template that ships inside the Transformation and Generative Tools tabs/panels respectively.
2. Take an existing Max for Live MIDI Tool and edit it.

Putting together a Max for Live MIDI Tool obeys the very same rules as making any other Max for Live device: with either a Max MIDI Transformation/Generator template chosen, or instead an existing Max for Live MIDI Tool, hit the Edit button to bring up the Max editor (“patcher”).

The Edit Button for a Max MIDI Transformation.

Once your edits are finished, the Save or Save As commands under the patcher’s File menu commit the Max for Live MIDI Tool to disk.

Out of the box, your computer keeps Max for Live MIDI Tools in the folders below:

- _Transformations_: ~/Music/Ableton/User Library/MIDI Tools/Max Transformations
- _Generators_: ~/Music/Ableton/User Library/MIDI Tools/Max Generators

As another option, the MIDI Tools’ AMXD files can sit in any folder listed under Places in Live’s browser. You might, say, make a fresh folder named “My Favorite MIDI Tools” and drop the Max for Live MIDI Tools you’ve built into it. Add that folder to Places in Live, and the MIDI Tools then show up across the drop-down menus of the Transformation/Generative Tools tabs/panels.

Keep in mind that Max for Live MIDI Tools kept somewhere other than the default location or Live’s Places escape Live’s Indexer, so they won’t turn up in the Clip View’s Transformation/Generative Tools tabs/panels.

To dig deeper into the Max objects behind Max for Live MIDI Tools, plus a step-by-step on patching a Max for Live Transformation or Generator, turn to the Max for Live MIDI Tools guide reachable through the Max documentation. From a Max window, choose Reference under the Help Menu, head to the Max for Live category, and open Guides.

### 31.5 Max Dependencies

As noted above, presets for Max devices bring a few unusual file-handling wrinkles. On top of that, the Max devices themselves might lean on additional files — samples, images, or even other Max patches — to function correctly. To tame these outside dependencies, Max for Live lets you [freeze](https://github.com/Ableton/maxdevtools/blob/main/m4l-production-guidelines/m4l-production-guidelines.md#freezing-and-dependencies) a Max device, and a frozen device packs in every file required to run it.

Be aware that freezing a Max device is _not_ the same thing as Live’s [Freeze Track](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#track-freeze) command.

For a deeper understanding of freezing and of how Max administers dependencies among its own files, the built-in Max documentation is the place to read.

### 31.6 Learning Max Programming

So that you can get further into making and editing Max devices, Cycling ’74 bakes thorough documentation and tutorials right into the Max environment. Open this material by picking “Reference“ from the Help menu in any Max window. A Max for Live section sits among the documentation contents as well.

The [Max for Live Production Guidelines](https://github.com/Ableton/maxdevtools/blob/main/m4l-production-guidelines/m4l-production-guidelines.md) documentation is another worthwhile read, hosted on GitHub.

If you’d rather learn by doing, grab the [Building Max Devices Pack](https://www.ableton.com/en/packs/building-max-devices/); its detailed lessons walk through every stage of assembling your own Max tools.

Beyond that, Cycling ’74’s [Learn Max page](https://cycling74.com/learn) gathers a broad set of learning resources worth exploring.
