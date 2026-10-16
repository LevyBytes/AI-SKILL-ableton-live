# Monitoring And External Audio Routing

Open when you need guidance on Monitoring And External Audio Routing in Ableton Live.

Context: [Routing and I/O](routing-and-i-o.md#17-routing-and-io).

<a id="source-171-monitoring"></a>
### 17.1 Monitoring

Inside Live, “Monitoring“ describes the act of routing a track’s incoming signal through to that track’s output. Imagine you have configured an audio track so its input arrives from a guitar. In that case, monitoring means the sound of your live guitar performance genuinely makes it to the track’s output by way of the track’s device chain. With the track’s output assigned to “Main,“ that guitar signal — shaped by whichever effects are in play (and pushed back by however much latency the audio hardware interface adds) — comes out of your speakers.

On each audio track and MIDI track, the In/Out section supplies a _Monitor_ radio button presenting these three choices:

-

For the majority of simple recording situations, the default _Auto_-monitoring setting behaves sensibly: it switches monitoring on while the track is [armed](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips), yet holds monitoring back whenever the track happens to be playing clips.

-

Selecting _In_ keeps the track’s input monitored at all times, no matter whether the track is armed or its clips are playing. In practice this makes the track behave like what certain systems label an “Aux“: rather than serving for recording, it brings a signal in from somewhere else. Under this choice, any output from the clips gets muted. You can spot an “In“ monitoring choice at a glance — even with the In/Out section collapsed — thanks to the blue color of the track’s Activator switch.

-

Picking the _Off_ option disables monitoring entirely. That comes in handy while recording acoustic instruments heard “through the air,“ while relying on an outboard mixing console to monitor, or while using an audio hardware interface whose “direct monitoring“ feature skips the computer to sidestep latency. As a rule, an audio interface capable of nearly imperceptible latencies (a few milliseconds) is the better choice. Should you record into Live with monitoring set to “Off,“ consider applying the Audio Settings’ Overall Latency adjustment, covered in the built-in program tutorial about configuring the Audio Settings.

With monitoring set to either “In” or “Auto,” the “Keep Monitoring Latency in Recorded Audio” option is on by default. It shifts the recording’s timing so it lines up with what you hear through Live’s monitoring. The usual advice is to keep this option on while recording software instruments or effects, and to turn it off while recording acoustic instruments or leaning on external monitoring. A right-click on the “In” or “Auto” monitor buttons lets you toggle “Keep Monitoring Latency in Record Audio” on or off by hand.

When several tracks are highlighted, clicking one of the Monitor buttons pushes that choice out to every selected track.

You can likewise bring the Monitor buttons back to how they began. While the In/Out section is open, press the Delete key, which restores each Monitor button to its default — that being “Off” on audio tracks and “Auto” on MIDI tracks — or instead choose the Edit menu option “Return to Default.”

<a id="source-172-external-audio-inout"></a>
### 17.2 External Audio In/Out

To pick the inputs of an audio interface, choose “Ext. In“ in an audio track’s Input Type chooser. From there, the Input Channel chooser presents the separate input channels. Each entry in that chooser carries a meter beside its label, which helps you spot whether a signal is present and whether it overloads (the meter turns red at that point). Configuring the audio interface’s outputs follows the same pattern through the output chooser pair. With several tracks highlighted, whatever edits you make in these choosers reach all of the selected tracks.

Which inputs and outputs show up is governed by the Audio Settings, reachable through the “Configure…“ option in the Input and Output Channel choosers. Bear in mind that the Audio Settings additionally open the Channel Configuration dialogs, which set which inputs and outputs are active and whether Live treats them as mono or as stereo pairs. In short, the Channel Configuration dialog supplies Live with the details it requires about how your computer hooks up to the rest of the audio gear in your studio.

Any input and output channels listed in the Channel Configuration dialogs may be renamed. Once you do, the revised name appears in the matching Input / Output Channel chooser drop-down. Renaming goes faster if you jump from one channel to the next with the Tab key. Keep in mind that a changed name stays tied to its particular audio device.
