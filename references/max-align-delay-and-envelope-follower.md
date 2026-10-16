# Max Align Delay And Envelope Follower

Open when you need guidance on Max Align Delay And Envelope Follower in Ableton Live.

Context: [Max for Live Audio Effects](max-for-live-devices.md#322-max-for-live-audio-effects).

<a id="source-3221-align-delay"></a>
### 32.2.1 Align Delay

The Align Delay Effect

A utility device, Align Delay holds back the signals coming into it by a measure given in samples, milliseconds, or meters/feet.

The Delay Mode drop-down menu offers three modes to pick from: Time, Samples, and Distance.

In Time mode the delay is expressed in milliseconds, which is handy for lining audio up with A/V equipment or for adding gentle stereo widening.

Samples mode states the delay in samples and serves to offset the latency that other devices introduce.

Distance mode gives the delay in meters or feet and is useful for fixing timing offsets that arise from the physical spacing of components in a PA system.

Distance mode also carries a Temperature option, comprising a toggle to pick Celsius or Fahrenheit alongside a slider that sets the temperature. Aligning these with the room's actual temperature sharpens the timing, since sound propagates at different rates in warm versus cold air.

Switch on the Link L/R toggle to copy the left channel's delay settings onto the right. With it active, the Delay Right slider is grayed out, and moving the Delay Left slider drives both channels together.

<a id="source-3222-envelope-follower"></a>
### 32.2.2 Envelope Follower

The Envelope Follower Effect.

As a modulator device, Envelope Follower reads the amplitude of whatever signal arrives and traces it as a smooth, continuous curve. That curve then drives whatever parameters you've mapped. One classic use of envelope following is the auto-wah.

Within Live, any automatable parameter — device or mixer controls among them — can be mapped to Envelope Follower. To do that, switch on the Map button and click a parameter to set it as the mapping target.

The Show/Hide Multimap button in the display's top-right corner reveals further mapping buttons, bringing the total you can map to eight.

You Can Map up to Eight Parameters.

Clearing an assignment is done with the Unmap button, found just to the right of the Map button.

Two routes exist for Envelope Follower to drive its mapped parameters: Modulation and Remote Control. The default is Modulation, though flipping the Mod toggle moves you to Remote Control.

With Modulation active, you remain free to change parameter values by hand even once they're mapped. The Modulation Polarity toggle flips between Bipolar and Unipolar modes. Under Bipolar, modulation swings both ways around a centered base value; under Unipolar, it moves in a single direction starting from the base value. The Modulation Amount slider fixes the modulation depth, defining the range relative to that base value.

Switch to Remote Control and the mapped parameter values are dictated entirely by Envelope Follower, with no manual adjustment possible. Scaling of the modulation range is handled by the Min and Max sliders.

The Gain knob applies gain to whatever signal comes in. Smoothing of the envelope's onset is handled by the Rise parameter, and smoothing of its tail by the Fall control — together these fine-tune the envelope's contour.

Delay time for the envelope is fixed by the Delay control. The Delay Mode buttons let you toggle between time-based delay and tempo-synced beat divisions.

By default, Envelope Follower derives its envelope from the track's own input signal. Turn on sidechain routing and it will instead read an external signal pulled from another track. As an example, sidechaining from a Drum Rack lets you build rhythmic ducking or gating effects.

The Sidechain Section in Envelope Follower.

The triangle toggle in the device's top-left corner unfolds the Audio Routing panel, where the sidechain controls live.

To configure sidechain routing, switch on the Sidechain toggle and pick the audio source from the first drop-down in the Audio From section. The second drop-down decides whether the signal is taken Pre FX, Post FX, or Post Mixer. When Racks are involved, you may also target a specific input channel.

Track-input and external-sidechain levels are shown respectively on the Direct and S.C. meters.

The Sidechain Mix control balances the track input against the external sidechain signal. Set to 0%, the envelope is built from the track input alone; set to 100%, it relies entirely on the external sidechain signal.
