# Routing And I O (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

#### 17.5.2.3 Creating Submixes

Submixing the separate drums of a kit.

Imagine that, for multitrack recording, each drum from a kit arrives on its own track. While tweaking the level of any single drum is trivial in that arrangement, balancing the whole kit against everything else in the song becomes awkward. The fix is to introduce a fresh audio track that acts as a submix for the drums. Each individual drum track is routed so that its output feeds this submix track, and the submix track in turn feeds the Main track. That single submix track then becomes a convenient level fader for the kit as a whole.

A different approach is to fold the separate drum tracks into a [Group Track](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks), which buys you additional flexibility. Doing so builds the required output routing on its own and lets you collapse or expand the tracks it contains.

Submixing by switching a track’s Output Type to Sends Only.

Yet another route relies on Live’s return tracks to do the submixing. Pick the Sends Only entry in a track’s Output Type and then raise a Send to taste. From that point on, the matching return track behaves as a submix channel.

#### 17.5.2.4 Several MIDI Tracks Playing the Same Instrument

Picture a MIDI track that holds a virtual instrument — say a Simpler producing a pad. After recording several MIDI clips onto this track, we decide we want a separate, parallel performance driven by that very same instrument. To make room for it, we create a second MIDI track. Dropping another Simpler onto the new track is one option, but our preference is to share the Simpler already living on the pad track, so that any edit to the pad’s timbre is heard across both tracks.

Routing one MIDI track into another so its instrument can be shared.

The way to do this is to point the new MIDI track’s Output Type chooser at the pad track. Observe that the Output Channel chooser then presents several possible targets: the new track’s signal can be routed into the pad track’s input, or it can be aimed straight at the Simpler. The “Track In“ choice in the Output Channel stands for the pad track’s incoming signal (what would get recorded), and that is not our aim. Instead we pick “Warm Bubbly Pad“ so that the new track’s MIDI lands on the Simpler directly, skipping the record and monitor path. Arranged this way, fresh takes can be captured on whichever track we like, and every one of them will sound the same pad.

The instrument now sits alone on its own track.

It may irritate us that silencing the pad track via its Activator switch also silences the other MIDI track. Strictly speaking the second track is still running, but the instrument voicing its MIDI has dropped out of the mix. The cure is straightforward: lift the clips off the pad track and drop them onto a third track that can be muted on its own (and that can carry its own MIDI effects). What remains of the original pad track is now nothing but a host for the instrument. Since no new clips will be captured on it, we can flip its Input Type chooser to “No Input,“ which hides its Arm button and cuts down on confusion whenever the mixer’s In/Out section is tucked away.

#### 17.5.2.5 Tapping Individual Outs From an Instrument

Certain software instruments — Live’s Impulse percussion sampler being one — provide several audio outputs for what they generate. Out of the box, Impulse folds its eight sample slots together internally and presents that blend at the instrument’s audio out, so any audio effect placed after Impulse on the same track acts on the combined signal. Now and then you may want to pull one drum hit clear of the blend for its own effects and balancing. That is feasible because Impulse exposes each of its sample slots as an audio source that other tracks can draw from.

Tapping Impulse’s separate outs to process sample slots on their own.

The procedure is simply to make an audio track and, from its Input Type chooser, point it at the track holding the Impulse. Alongside Pre FX, Post FX and Post Mixer, the Input Channel chooser then lists Impulse’s eight separate outputs, each named after the sample loaded in that slot. Bear in mind that pulling one of Impulse’s outputs into a different track removes that signal from Impulse’s own internal blend automatically. That handy behavior is not what most plug-in instruments do by default, though. Soloing whichever track taps one of Impulse’s slots still lets you monitor what that slot produces.

#### 17.5.2.6 Using Multi-Timbral Plug-In Instruments

Plenty of plug-in instruments can run in multi-timbral mode. Such an instrument behaves as though it were a stack of instruments bundled together, where each constituent “part“ (or whatever label the maker prefers) listens for MIDI on its own MIDI channel. As a rule, a multi-timbral instrument hands you separate outputs so each part can be routed into the mixer independently, or it bundles a submixer inside itself.

Tracks sending MIDI to, and pulling audio from, the parts of a multi-timbral instrument.

Delivering MIDI from the mixer into a multi-timbral instrument is just a twist on a [case described above](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#several-midi-tracks-playing-the-same-instrument). A single MIDI track carries the multi-timbral instrument while further MIDI tracks supply its individual parts. On each of those extra MIDI tracks, the Output Type chooser is aimed at the track holding the instrument and the Output Channel chooser names the MIDI channel you intend to drive. From there, extra audio tracks can pull the instrument’s separate outputs, exactly as [described earlier](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#tapping-individual-outs-from-an-instrument).

The External Instrument device can likewise carry MIDI to (and bring audio back from) the auxiliary outputs of multi-timbral plug-ins. With this approach there is no longer any need to spin up a separate audio track for every output you tap:

1. Place the multi-timbral instrument onto a MIDI track.
2. Drop an External Instrument device onto a second MIDI track.
3. In the first MIDI To chooser on the External Instrument device, pick the track that holds the instrument.
4. Using the second chooser on the External Instrument device, choose the MIDI channel you want to address.
5. From the External Instrument’s Audio From chooser, pick an auxiliary output belonging to the instrument you are feeding MIDI.

Run through steps 2-5 again for each further part of the multi-timbral instrument you wish to feed and tap. The whole arrangement of External Instrument devices can even live on one track if you slot each into the device chain of a Rack.

Keep in mind that the multi-timbral instrument’s primary outputs continue to feed the track holding the instrument — the External Instrument device only ever reaches the auxiliary outputs.

#### 17.5.2.7 Feeding Sidechain Inputs

Certain effects come with what are termed “sidechain inputs.“ Take a vocoder: it stamps the spectral profile of one source (spoken word, perhaps) onto a second source, such as a string pad. You place the vocoder as an audio effect on the string track, and its sidechain input expects the speech signal, which must arrive from somewhere else. To supply it, we build an extra audio track called “Speech,“ aim its Output Type chooser at the “Strings“ track, and from the Output Channel chooser pick the vocoder’s sidechain input.

A handful of vocoder plug-ins bundle a synthesizer to produce the “carrier“ themselves. The only thing that changes here from the steps just given is that the vocoder instrument goes onto a MIDI track. Routing audio into the sidechain input proceeds just as before.

Several of Live’s native devices ship with their own sidechain sections whose routing choosers mirror those on tracks. When you work with one of these devices, there is no reason to walk through the steps above — the sidechain source can be chosen right inside the device.

#### 17.5.2.8 Layering Instruments

Say we have a MIDI track whose instrument is producing a string sound, and we want to thicken it with a brass sound sounding the very same notes. The simple solution is to add a MIDI track holding an instrument that plays the brass sound, then set its Input Type chooser so it taps the string track’s Post FX signal.

Layering instruments by way of a helper MIDI track.

You may be puzzled that this functions at all, considering the string track puts out audio rather than MIDI. The trick is that when MIDI is routed in from another track, it is grabbed at the very last point possible — past any MIDI Effects and immediately before the instrument.
