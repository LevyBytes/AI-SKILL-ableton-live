# Rack Chain Select Preset Banks

Open when you need guidance on Rack Chain Select Preset Banks in Ableton Live.

Context: [Chain Select Zones](instrument-drum-and-effect-racks.md#2454-chain-select-zones).

<a id="source-24541-making-preset-banks-using-chain-select"></a>
#### 24.5.4.1 Making Preset Banks Using Chain Select

Using Chain Select Zones to Create Effects Presets.

In contrast to the other zone types, a chain select zone starts out with a length of 1 and a value of 0. Beginning from that arrangement, the Chain Select Editor lets us whip up “preset banks“ in short order.

Once more, let’s take a Rack holding four chains as our point of departure. The four chains each house a different set of effects that we’d like to flip among. So that this feels truly “hands-on,“ we’ve gone ahead and MIDI-mapped the Chain selector onto an encoder on an external control surface.

Let’s shift the chain select zones belonging to the second and third chains so that every zone lands on its own neighboring value: the first chain’s zone sits at 0, the second chain’s zone at 1, the third at 2, and the fourth at 3.

Because every one of our chain select zones now holds a distinct value and none of them overlap, we’ve arrived at a state in which just a single chain can ever match the Chain selector value (displayed across the editor’s top) at any given moment. As a result, sliding the Chain selector is what decides which chain gets to process signals. With our MIDI encoder ready to go, switching between instrument or effect setups becomes wonderfully easy.

<a id="source-24542-crossfading-preset-banks-using-fade-ranges"></a>
#### 24.5.4.2 Crossfading Preset Banks Using Fade Ranges

Crossfading Between Effects Presets Using Chain Select Zones.

Pushing the earlier example a notch further, we can adjust our chain select zones so they glide smoothly from one of our “presets“ to the next. Pulling that off means putting our zones’ _fade ranges_ to use.

So there’s space for fading to happen, let’s stretch our zones out a little. Arranging the zones the way shown keeps four exclusive values for the presets intact, ensuring each one still has a spot where none of the others sound. The crossfade between presets unfolds across eight steps. Should that prove too abrupt for your material, just reposition the zones to make the fade ranges as wide as possible.
