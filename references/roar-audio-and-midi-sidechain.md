# Roar Audio And MIDI Sidechain

Open when you need guidance on Roar Audio And MIDI Sidechain in Ableton Live.

Context: [Roar](redux-resonators-reverb-and-roar-routes.md#2833-roar).

<a id="source-28336-sidechain-parameters"></a>
### 28.33.6 Sidechain Parameters

Out of the box, Roar relies on its own input signal both to feed its envelope follower and to determine its feedback pitch. With the Sidechain section, however, you can substitute external audio and MIDI signals for that role. Reveal the external and MIDI sidechain controls by clicking the Sidechain Section toggle located at the device’s top-left corner.

Roar’s Sidechain Parameters.

Turn on the External SC toggle to activate the external sidechain. After it is enabled, the External Source chooser lets you point to whichever signal you want to use. The External Tapping Point chooser additionally controls whether that signal arrives Post FX or Post Mixer.

With the Mix slider, you can blend the external and internal sidechain signals together so they jointly act as the envelope follower’s trigger. Setting it to 100% makes the envelope follower follow only the external sidechain source, whereas at 0% just the internal sidechain feeds it.

Adjust the incoming level of the external sidechain through the SC Gain control. Keep in mind that this sidechain audio serves purely as a trigger for the envelope follower, so raising the gain has no bearing on how loud the source signal sounds.

Enable the MIDI > FB Note toggle so that MIDI input governs the pitch of Roar’s feedback engine whenever the [feedback mode](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#feedback-section) is configured to Note. After the MIDI sidechain is on, the External Source chooser found beneath MIDI From selects which MIDI sidechain source is used. The Tapping Point chooser likewise sets whether the signal is captured Pre FX or Post FX.

Be aware that while the MIDI sidechain is engaged, the Feedback Mode and Feedback Amount controls within the [feedback section](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#feedback-section) become inactive.

Activate the Sidechain Listen toggle to audition the sidechain signal on its own. Doing so mutes Roar’s normal output so you can listen straight to the sidechain input, which comes in handy while you dial in the sidechain settings.

The Sidechain Listen Toggle.
