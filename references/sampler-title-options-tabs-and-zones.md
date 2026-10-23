# Sampler Title Options Tabs And Zones

Open when you need guidance on Sampler Title Options Tabs And Zones in Ableton Live.

Context: [Sampler](operator-and-sampler-routes.md#3010-sampler).

<a id="source-30103-title-bar-options"></a>
### 30.10.3 Title Bar Options

Sampler’s Title Bar Context Menu.

Before we dive into the rich modulation capabilities Sampler offers, it's worth surveying the entries available in its title bar context menu.

While Cut, Copy, Rename, Edit Info Text, and Delete are likely things you already recognize, a few of the remaining choices warrant a closer look:

_Group_: Choosing this option places Sampler inside a fresh Instrument Rack.

_Fold_: Collapses Sampler down to just its device title bar. A quick double-click on that title bar brings it back open again.

_Show Preset Name_: Normally, Sampler adopts the name of the uppermost sample in the sample layer list for its title. Turn off Show Preset Name and the title becomes “Sampler.” instead.

_Lock to Control Surface_: Ties Sampler to a control surface that Live natively supports, as configured in the Link, Tempo & MIDI Settings, so you keep direct control regardless of what currently has focus in your Live Set. Whenever a track is armed for recording, Sampler locks to the control surface on its own by default. To signal this state, a hand icon appears in the title bar of any locked device.

_Save as Default Preset_: Stores Sampler’s present configuration to serve as the default preset.

_Use Constant Power Fade for Loops_: Out of the box, Sampler applies constant-power fades where loops meet. Disable this option and looping points instead receive linear crossfades.

_Sampler -> Simpler_: Translates Sampler presets into [Simpler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#simpler) presets. That makes it simple to pass Sets along to collaborators whose Live edition lacks Sampler.

<a id="source-30104-samplers-tabs"></a>
### 30.10.4 Sampler’s Tabs

Sampler’s Tabs in the Title Bar.

Reachable from Sampler‘s title bar, Sampler’s capabilities are grouped by category across a set of tabs: Zone, Sample, Pitch/Osc, Filter/Global, Modulation and MIDI. Selecting a tab exposes the relevant properties underneath it — the lone exception being the Zone tab. Beyond just keeping things tidy, each tab carries one or more LEDs that light up to show whether modulation data exists in that section. Our tour of Sampler proceeds tab by tab.

<a id="source-30105-the-zone-tab"></a>
### 30.10.5 The Zone Tab

The Zone Tab.

Selecting the Zone tab switches Sampler‘s Zone Editor on or off. That editor gives you a direct, visual way to assign any quantity of samples across three kinds of ranges, handled by the Key Zone, the Velocity Zone and Sample Select Editors in turn.

The Key Zone Editor.

Rather than sharing space, the Zone Editor appears in its own view positioned immediately above the Device View. Paired with Sampler’s remaining tabs, this arrangement makes building and tweaking multisamples considerably faster.

Running down the left edge of the Zone Editor sits the sample layer list, which keeps multisamples organized. Each separate sample that makes up a multisample appears in this list, and here such samples carry the name _layers_. With intricate multisamples, the list may grow rather lengthy.

Sitting just above the sample layer list is a row of buttons used to set up the sample layers and switch among the various editors:

_Auto Select (Auto)_: When MIDI notes reach Sampler, each one passes through the key, velocity and sample select zones belonging to every sample layer. Turn on Auto Select and every sample layer capable of sounding an arriving note gets highlighted in the sample layer list for as long as that note lasts.

_Zone Fade Mode (Lin/Pow)_: Pressing this button switches the fade slope of all zones back and forth between linear and constant-power (exponential).

_Round Robin (RR)_: Use this button to switch [Round Robin sample playback](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#round-robin-sample-playback) either on or off.

_Zone Editor View (Key/Vel/Sel)_: These buttons control whether the Key Zone, Velocity Zone and Sample Select Editors are shown.

Filling the remainder of the view is whichever of three sample-layer editors is active: the [Key Zone Editor](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#key-zones), the [Velocity Zone Editor](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#velocity-zones) and the [Sample Select Editor](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sample-select-zones). To adjust their horizontal zoom, right-click inside one to open a context menu and pick Small, Medium or Large.
