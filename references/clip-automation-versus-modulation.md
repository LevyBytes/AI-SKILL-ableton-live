# Clip Automation Versus Modulation

Open when you need guidance on Clip Automation Versus Modulation in Ableton Live.

Context: [Clip Envelopes](clip-envelopes.md#26-clip-envelopes).

<a id="source-263-mixer-and-device-clip-envelopes"></a>
### 26.3 Mixer and Device Clip Envelopes

You can press clip envelopes into service to _automate_ or _modulate_ mixer and device controls. Because such controls might be driven by both envelope types simultaneously (and on top of that by the Arrangement's [automation envelopes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation), some confusion can creep in. There is, though, one key respect in which modulation envelopes part ways with automation envelopes: an automation envelope fixes the absolute value a control holds at each moment, whereas a modulation envelope can merely nudge that already-set value. That distinction is what lets the two kinds cooperate smoothly even when they act on the same parameter. As a visual cue, automation envelopes are drawn in red and modulation envelopes in blue. On parameters that use knob controls, automation shifts the absolute position (the “needle”), while modulation shows up as the blue segment around the ring.

Suppose you've captured volume automation on an audio clip that steadily fades it out across four bars. Now what becomes of that fade-out once you add a modulation envelope that steadily lifts the mixer volume over those same four bars? Early on, the fade-out turns into a swell, since the modulation envelope keeps pushing the volume up as far as the automation envelope permits. Yet as soon as the falling automated value crosses paths with the rising modulation value, the fade-out kicks in, because automation drives the absolute control value — and with it the working range of the modulation envelope — downward.

Clips in the Session View offer both automation and modulation clip envelopes. Sitting below the envelope choosers, a toggle lets you flip between editing the automation and the modulation clip envelope for whatever parameter you've chosen. Over in the Arrangement, clips carry modulation envelopes alone, with their automation envelopes living on the track's [automation lane](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation).

Toggle Between Editing Automation and Modulation Envelopes.

Within a clip, any parameter carrying an automation envelope is flagged by a red LED in the Control chooser, and likewise a blue LED marks one carrying a modulation envelope. A parameter may show both a red and a blue LED at once, signaling that the clip is automating and modulating it together.

LEDs Indicate Existing Automation and Modulation Envelopes for the Selected Parameter.
