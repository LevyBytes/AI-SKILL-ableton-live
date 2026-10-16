# Preset Saving And Defaults

Open when you need guidance on Preset Saving And Defaults in Ableton Live.

Context: [Using Devices](working-with-instruments-and-effects.md#232-using-devices).

<a id="source-2325-saving-presets"></a>
### 23.2.5 Saving Presets

In the browser’s _User Library_, you’re free to build and store as many of your own presets as you like.

The Save Preset Button.

Hit the Save Preset button to keep a device’s current settings (custom info text included) as a brand-new preset. Live then takes you to the browser, where pressing Enter accepts Live’s proposed name or you can enter your own. Press the Esc key to back out of saving. You can also drop presets into particular folders in the browser’s Places section (for example, your Current Project folder) by dragging from the device’s title bar into whichever browser spot you choose.

For a thorough rundown of what the browser can do, see the [Managing Files and Sets](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#managing-files-and-sets) chapter. To learn about keeping presets tied to a specific project, see the [Projects and Presets](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#projects-and-presets) section.

<a id="source-2326-default-presets"></a>
### 23.2.6 Default Presets

Whenever you store presets in the _Defaults_ folders inside your User Library, they take the place of the standard device settings when loading. The Defaults folders additionally let you:

- Tailor Live’s behavior toward various user actions, like dropping samples, slicing, and converting audio to MIDI.
- Make freshly created MIDI and audio tracks open with specific devices already loaded and their parameters set the way you want.
- Open VST and Audio Units plug-ins with a chosen set of parameters already laid out in Live’s panel.
  The Default Presets folders in the User Library.

To store a Live device’s current settings as a default preset, bring up the context menu on the device’s header and choose “Save as Default Preset.“ It applies to every one of Live’s instruments, MIDI effects, and audio effects (the various [Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks) included). When a default preset already exists for that device, Live prompts you before replacing it.

To build a default configuration preset for a VST or Audio Unit plug-in:

- Load the chosen plug-in onto a track.
- Within the plug-in’s [Configure Mode](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#plug-in-configure-mode), arrange the set of parameters you want.
- Bring up the context menu on the track header and choose “Save as Default Configuration.”

When both the VST and Audio Units builds of a given plug-in are installed, you can make a separate default configuration preset for each one. Note that a plug-in’s default preset doesn’t store the _settings_ of the configured parameters; what gets saved is only how the parameters are arranged in Live’s panel.

To build default presets for MIDI and audio tracks:

- Place whatever device(s) you want as the default onto a track (or none at all, if your default track should be empty).
- Set the device parameters however you prefer.
- Bring up the context menu on the track header and choose “Save as Default Audio/MIDI Track.”

To set how Live responds when you drag a sample to a Drum Rack or to the Device View of a MIDI track:

- Make an empty Simpler or Sampler.
- Set the parameters however you prefer.
- Drag the adjusted device onto the “On Drum Rack“ or “On Device View“ folder inside the Defaults/Dropping Samples folders of your User Library. You can also store Drum Rack pad defaults through a context menu option on a Drum Rack’s pad.

To change how Live responds when slicing an audio file:

- Make an empty Drum Rack.
- Put an empty Simpler or Sampler into the Drum Rack so there’s a single chain.
- Add whatever extra MIDI or Audio Effects you want to this chain.
- Set the parameters on any of the devices.
- Map [Macro Controls](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#using-the-macro-controls) to any of the controls in the chain’s devices.
- Drag the whole Drum Rack onto the Defaults/Slicing folder of your User Library.

You’re free to make several slicing presets and pick among them using the Slicing Preset chooser in the slicing dialog.

To build default presets for [converting Drums, Harmony, or Melody to MIDI](https://www.ableton.com/en/live-manual/12/converting-audio-to-midi/#convert-harmony-to-new-midi-track):

- Make a MIDI track holding the instrument you want as the default for a given conversion type. Note that a default preset for converting drums has to include a Drum Rack.
- Add whatever extra MIDI or Audio Effects you want to the track.
- Set the parameters on any of the devices.
- When you’re using more than one device, bundle them into a Rack.
- Drag the whole Rack onto the matching folder in Defaults/Audio to MIDI of your User Library.

Beyond these application-wide default presets, you can also make default presets that apply to a single Project only. That comes in handy when, say, you rely on tailored device or track setups for one particular Set and want to spin off variations of the Set that still have these presets, all without disturbing the broader default presets you use elsewhere. To build Project-specific default presets:

<a id="source-working-with-instruments-and-effects-part-2"></a>

- Rebuild the Defaults folder inside the Project folder, along with whatever subfolders you want.
- Set the relevant device parameters, track settings, and so on, based on the kinds of Project-specific defaults you intend to use.
- Store the device or track in the matching folder under your Project-specific Defaults folder.

From then on, loading a Set belonging to this Project will pull any default presets you stored in these Project folders rather than the ones in the User Library. Keep in mind that the context menu commands for saving defaults route them to your primary User Library, which means they can't create Project-specific defaults.
