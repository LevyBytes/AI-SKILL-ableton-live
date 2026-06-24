# Computer Audio Resources And Strategies

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 37. Computer Audio Resources and Strategies

Processing sound in real time places heavy demands on everyday computers, machines typically built for office work and web browsing rather than audio. Running Live well calls for a capable CPU paired with a quick SSD. The pages that follow offer guidance for preventing and fixing the resource bottlenecks that can crop up while you work in Live.

### 37.1 Managing the CPU Load

Delivering an unbroken flow of audio out to the hardware forces Live to run an enormous quantity of math each second. Should the processor fall behind on that workload, you will end up with clicks or dropouts in the sound.

Several things shape how fast a machine can compute: the processor clock rates (e.g., speed in MHz or GHz), the chip architecture, the temperature (when it gets too warm, today's CPUs “thermal throttle” by dialing back their pace), the memory cache performance (a measure of how readily the chip pulls data out of memory), and the system bus bandwidth — the computer’s “pipeline“ that every byte has to travel along.

The good news is that Live works with multicore and multiprocessor systems, so the workload from instruments, effects, and I/O can be spread across the resources you have on hand. The usable processing power may exceed that of older machines by a wide margin, depending on your hardware and the Live Set in question.

### 37.1.1 The CPU Load Meter

How much of your machine's compute capacity is in use at the moment is shown by the CPU meter in the Control Bar. A reading of 10 percent, say, means the computer is barely working. Once it reaches 100 percent the processor is fully saturated, and at that point clicks, gaps, or similar audio glitches become likely.

Keep in mind that this meter reflects solely the burden of audio processing and ignores everything else the machine handles (e.g., managing Live’s user interface).

The CPU load meter shown.

You can set this meter to show Average or Current CPU usage, or turn it off completely.

In Average mode, the meter reports the mean share of the CPU devoted to audio at the moment, not the system-wide CPU load. The Current CPU meter, by contrast, reports the full present CPU usage.

Clicking the CPU meter brings up its assorted settings.

The CPU Load Meter Options.

Out of the box, the Current level stays hidden in Live and has to be turned on through the drop-down menu.

Fresh setups of Live 11 likewise ship with the CPU Overload Indicator turned off. Whenever you want it back, choose Warn on Current CPU Overload from the drop-down menu to re-enable it.

Live works out the CPU load by timing how long it takes to crunch a single audio buffer. It then weighs that figure against how long playing one audio buffer actually lasts.

So a reading of 50% on the meter indicates that Live chews through one audio buffer in half the time the buffer needs to play.

Readings above 100% can occur whenever the math runs longer than the playback of a single audio buffer.

Although Live assumes its audio thread should run at top priority, the operating system has the last word on how threads are ranked, so Live’s work can be cut into. That is the reason other programs sometimes show up as CPU spikes on Live’s CPU meter.

### 37.1.2 CPU Load from Multichannel Audio

Shuttling data back and forth between the software and the audio hardware is one steady source of CPU drain. You can trim that cost by switching off whichever inputs and outputs a project doesn't use. The Audio Settings hold two buttons that open the Input and Output Configuration dialogs, where individual ins and outs can be turned on or off.

Channels you aren't using stay enabled on their own, since asking the audio hardware drivers to change configuration tends to cause a noticeable “hiccup“ in the sound.

### 37.1.3 CPU Load from Tracks and Devices

As a rule, each active track and device in Live adds a bit of CPU load. Even so, Live is “smart“ enough not to burn CPU cycles on any track or device that isn't actually doing useful work.

To illustrate, dropping devices into a Live Set while it sits idle barely moves the CPU load. That load climbs only once clips begin playing or audio reaches the effects. With nothing coming in, the effects shut down until called for again. For an effect that leaves a “tail,“ like reverbs and delays, that shutdown waits until every calculation has finished.

This approach trims the average CPU load of a Live Set quite well, yet it does nothing for the peak load. To confirm your Live Set will keep playing without interruption even at its busiest, trigger a clip on every track at once while all devices are switched on.

Within the Session View, you can reveal how each track weighs on the CPU by clicking the Show/Hide Performance Impact selector found in the Mixer Section.

The Show/Hide Performance Impact selector.

Inside the Performance Impact section, every track carries a dedicated CPU meter made of six rectangles, which illuminate to show how heavily that track weighs on the CPU level of the current Set. [Freezing the track](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#track-freeze) that weighs the most, or stripping devices off it, will typically bring the CPU load down.

The Session View’s Performance Impact Section.

### 37.1.4 Track Freeze

When devices and clip settings pile CPU load onto a track, Live‘s Freeze Track command is a strong remedy. Pick a track, run the Freeze Track command, and Live builds a sample file for every Session clip on that track along with one for the Arrangement. From then on, the track's clips merely replay these “freeze files“ instead of endlessly recomputing demanding device and clip settings on the fly. You can reach the Freeze Track command through Live‘s Edit menu as well as the context menu on tracks and clips. Note that a [Group Track](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks) cannot be frozen; freezing only works on tracks that contain clips.

In most cases freezing finishes almost instantly. The exception is a track holding an [External Audio Effect](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#external-audio-effect) or [External Instrument](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#external-instrument) routed out to a hardware effects unit or synth, where the freeze must run in real-time. Live spots on its own whether real-time freezing applies, then offers you a handful of choices for handling it. For a rundown of those choices, consult the section on [real-time rendering](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#real-time-rendering).

After you've dealt with the processing burden (or perhaps bought a faster computer!), you're free at any time to highlight a frozen track and pick Unfreeze Track from the Edit menu so you can adjust device or clip settings. With a slower rig, it helps to unfreeze demanding tracks individually for editing, then freeze each one again once you've finished.

A frozen track still grants access to plenty of editing operations. You can fire off clips as usual, and mixer controls like volume, pan, and the sends stay within reach. The list also covers:

- Trim, cut, copy, paste, duplicate, and otherwise edit clips.
- Draw and adjust mixer automation along with mixer clip envelopes.
- Merge clips together via Consolidate.
- Capture Session View clip launches as Arrangement View recordings.
- Build, relocate, and duplicate scenes in the Session View.
- Pull frozen MIDI clips over onto audio tracks.

If you edit a frozen track carrying time-based effects like reverb, bear in mind that what you hear could shift once the track is unfrozen again, depending on the case. The reason is that a frozen track's effects aren't being computed whatsoever, so they can't adapt their response to the material you've changed. Unfreezing the track triggers all of those effects to be recomputed live.

A Frozen Arrangement Track with a Reverb Tail.

In the Arrangement View, frozen tracks still sound any pertinent material that runs past where their clips end (e.g., the “tails“ of Reverb effects). Such frozen tails show up in the Arrangement as crosshatched areas sitting right next to the clips they belong to. Live regards them as standalone, “temporary“ clips that vanish on unfreezing, because the effect gets computed live at that point. For this reason, when you reposition a frozen clip in the Arrangement, it's usually wise to grab the accompanying frozen tail clip too, keeping the pair together.

A frozen Session clip captures just two loop cycles, so clips that use [unlinked clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#unlinking-clip-envelopes-from-clips) can sound different once those two loop cycles pass while frozen.

Drop a frozen clip onto the drop area in either the Session View or Arrangement View and Live spins up a fresh frozen track holding that clip. Should only part of a clip be selected in the Arrangement, the new frozen track captures just that selected stretch.

Whatever samples the Freeze Track command produces land inside the Current Project folder at /Samples/Processed/Freeze. When the Set hasn't been saved yet, that destination is set instead by the [Temporary Folder](https://www.ableton.com/en/live-manual/12/recording-new-clips/#where-are-the-recorded-samples). Keep in mind that freeze files belonging to tracks with an External Instrument or External Audio Effect get thrown away the instant you unfreeze.

Beyond saving CPU on tracks stuffed with many devices, the Track Freeze command makes it easier to move projects from one computer to another. A machine that's somewhat short on horsepower can still handle sizeable Live Sets provided the heavy tracks are frozen. By the same token, a computer that doesn't have certain devices from a Live Set can nonetheless play that Set once the tracks using those devices are frozen.

### 37.2 Managing the Disk Load

How quickly an SSD reads and writes has a bearing on how Live performs. The volume of disk traffic Live creates scales more or less with how many audio channels are being read or written at the same time. To take one case, a track sounding a stereo sample drives more disk traffic than one sounding a mono sample.

The Disk Overload Indicator.

Whenever the disk fails to read or write audio fast enough, the Disk Overload indicator blinks. While you're recording, that situation leaves a gap in the captured sample; during playback, it surfaces as dropouts.

To steer clear of disk overload, try these steps:

- Cut how many audio channels you write by picking mono inputs over stereo inputs within the Audio Settings’ Channel Configuration dialog.
- Switch on [RAM Mode](https://www.ableton.com/en/live-manual/12/clip-view/#clip-ram-mode) for the clips you choose.
- Lower the count of audio channels in playback by favoring mono samples over stereo samples wherever you can. Turning a stereo sample into mono is doable in any ordinary digital audio editor, which you can launch [from within Live](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#viewing-and-changing-a-live-sets-file-references).
