# Hybrid Reverb Routing And Engines

Open when you need guidance on Hybrid Reverb Routing And Engines in Ableton Live.

Context: [Hybrid Reverb](gate-glue-grain-hybrid-reverb-routes.md#2823-hybrid-reverb).

<a id="source-28231-signal-flow"></a>
### 28.23.1 Signal Flow

Picture the audio moving through Hybrid Reverb from the device’s left edge toward its right, entering the input section first and then reaching the reverb engines. How those two engines relate to one another is shaped by the routing section; from there the signal travels through the EQ section before it arrives at the output.

On the interface, the convolution reverb engine’s controls are colored yellow, whereas the algorithmic engine’s controls show up in blue.

<a id="source-28232-input-section"></a>
### 28.23.2 Input Section

The Send knob lets you dial in how much gain is applied to the signal driving the reverb. Keep in mind the dry signal stays untouched and continues to flow through the device.

How long the device waits before the first early reflection appears is set by Predelay, which pushes the reverberation back in time relative to the input. Part of how large a real space seems comes from this gap; for “natural” results, figures from 1ms to 25ms are typical. The Predelay Sync buttons let you pick either a time-based predelay or one synced to the beat.

Feedback determines how much of the predelay’s output is returned to its own input. Note that the time-based and beat-based predelay modes each carry their own separate feedback setting.

Hybrid Reverb’s main window holds two tabs, Reverb and EQ. Every control tied to both the convolution and algorithmic engines lives under the Reverb tab. Beginning with the Routing chooser at the center, four choices are available:

- Serial feeds the convolution engine’s output into the algorithmic engine. The convolution reverb stays on at all times here, while Blend sets how much of it is passed along to the algorithmic reverb. At 100/0 you get convolution reverb alone, and at 0/100 you get purely algorithmic reverb that has been driven by the convolution reverb’s output.
- Parallel runs both the convolution and algorithmic engines but keeps them apart from each other. Here the Blend knob sets the level balance between the two engines, with 100/0 yielding only convolution reverb and 0/100 yielding only algorithmic reverb.
- Algorithm engages the algorithmic reverb engine by itself.
- Convolution engages the convolution reverb engine by itself.

The interface of Hybrid Reverb adapts on the fly, so any engine that isn’t currently active will have its controls dimmed out.

When Routing is set to Serial or Parallel, the Blend knob crossfades between the convolution and algorithm section outputs. Bear in mind that picking either Algorithm or Convolution in the Routing chooser leaves the Blend knob with nothing to do.

<a id="source-28233-convolution-reverb-engine"></a>
### 28.23.3 Convolution Reverb Engine

Hybrid Reverb’s Convolution Reverb Section.

To produce its effect, a convolution reverb relies on recordings of real spaces, known as impulse responses. That lets you situate your sounds inside nearly any environment you happen to have a recording of. For more conventional reverb, that might mean some of the world’s most renowned halls and studios. Take a more experimental route and you could use recordings of just about anything — snare drums, garbage cans, even instrumental or vocal takes!

You select impulse responses from the Convolution IR menu. The top drop-down picks the impulse response category, and the bottom drop-down selects a particular impulse response inside that category. Backward and forward arrow buttons make browsing the impulse responses easy. Once you hit the end of a category, these arrows roll over to the next one automatically, letting you sweep through every impulse response with the arrows by themselves. The selected impulse response’s waveform then appears in the main display, which redraws according to the Attack, Decay, and Size settings (covered below).

Several impulse response categories are provided. The first few cover Early Reflections, Real Places, and Chambers and Large Rooms. After those come Made for Drums, then Halls, Plates and Springs. Rounding out the set are Bigger Spaces, Textures, and finally User.

To load your own impulse responses into the User category, drag and drop the IR audio file onto Hybrid Reverb’s convolution waveform display. Should you drop in a file from a folder holding other audio files, every one of them gets added as an impulse response. Note: take Hybrid Reverb off a track and put it back, and any User samples you’d added before will be gone from the User category. You can, though, drag and drop those samples onto the waveform display once more to rebuild the list.

The impulse response’s amplitude envelope is governed by the Attack, Decay, and Size parameters. Attack sets the envelope’s attack time, Decay sets its decay time, and the Size parameter changes the impulse response’s relative size.

<a id="source-28234-algorithmic-reverb-engine"></a>
### 28.23.4 Algorithmic Reverb Engine

Hybrid Reverb’s Algorithmic Reverb Section.

Unlike the convolution engine, the algorithmic engine rests entirely on digital delay lines and draws on no samples whatsoever.

The controls for the algorithmic reverb engine sit to the right of the Blend knob. Which parameters appear there depends on the selection you make in the Algorithm chooser.

You have five algorithms to choose from: Dark Hall, Quartz, Shimmer, Tides and Prism. Across every one of them, the Decay, Size, Delay and Freeze parameters are present.

Decay sets roughly how long the algorithm’s reverb tail takes to fall to 1/1000th (-60 dB) of where it started. Size dictates how big the virtual room is. Delay tacks on an extra predelay, in milliseconds, for the algorithm section.

Two buttons, Freeze and Freeze In, make up the Freeze controls. Freeze cuts off all input to the reverb engine and stretches the algorithm’s decay to infinite, so the reverb output carries on without end. Switching on Freeze In folds the input signal into the frozen reverberation, which builds up an accumulating wash of reverb.

Below, each algorithm and the parameters unique to it are explained in more depth.
