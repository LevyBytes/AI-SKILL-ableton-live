# Collision Resonator Models And Decay

Open when you need guidance on Collision Resonator Models And Decay in Ableton Live.

Context: [Collision](analog-and-collision-routes.md#302-collision).

<a id="source-3024-resonator-tabs"></a>
### 30.2.4 Resonator Tabs

Collision’s Resonators.

What gives Collision most of its personality are the controls living in its pair of Resonator tabs. A switch inside each tab flips that resonator on or off. Be aware that switching both resonators off yields silence.

Up at the head of the Resonator tab there is a Resonance Type drop-down listing resonant objects:

- Beam reproduces how beams made of assorted materials and sizes resonate.
- Marimba is a tailored offshoot of the Beam model that captures how marimba bar overtones are tuned — a quality stemming from the bars’ pronounced arch-cut underside.
- String mimics the tone of strings built from assorted materials and sizes.
- Membrane represents a rectangular membrane — a drum head, say — whose dimensions and build can be varied.
- Plate emulates the sound made by a rectangular plate, that is a flat sheet, across assorted materials and sizes.
- Pipe represents a cylindrical tube left fully open on one side with an adjustable aperture on the other (set through the Opening parameter.)
- Tube represents a cylindrical tube sealed at each end.

Picking an object places a depiction of it onto the X-Y Controller display.

Beside the Resonance Type drop-down lies a Quality menu offering settings from Eco through to High. By cutting how many overtones get computed, Quality balances resonator fidelity against CPU load. Choosing Eco keeps CPU demand low, whereas High yields richer resonances. Bear in mind that no Quality menu appears for the Pipe or Tube resonators.

A copy button sits inside each resonator (labeled 1 → 2 within Resonator 1 and 2 → 1 within Resonator 2), letting you transfer every setting from one resonator over to its counterpart.

With the X-Y Controller, dragging the mouse left-to-right alters the resonant object’s decay time, and dragging up-and-down alters the Material/Radius parameter.

Internal damping inside the resonator is what decay time governs, and the Decay slider provides another way to set it.

How damping varies from one frequency to the next is set by the Material slider. With lower settings, the low-frequency content fades more gradually than the high-frequency content (the behavior of wood, rubber, or nylon objects). With higher settings, it is the high-frequency content that lingers longer (the behavior of glass or metal objects).

For the Pipe and Tube resonators, a Radius parameter takes the slot the Material parameter would otherwise hold. That slider governs how wide the pipe or tube is. A growing radius lengthens both the decay time and the high-frequency sustain. Push the size very large and the resonator’s fundamental pitch shifts as well.

Note pitch and velocity can drive the Decay and Material/Radius parameters by way of the Key and Vel sliders on the MIDI tab.

For the Membrane and Plate resonators only, a Ratio parameter appears that controls how the object’s dimensions compare along its x and y axes.

How loud the various frequency components are is governed by the Brightness control. Crank it up and the upper frequencies grow louder. The Pipe and Tube resonators ignore this parameter.

Pitch of the resonator’s harmonics is shifted by the Inharm knob. Drive it negative and the frequencies bunch together, swelling the count of lower partials. Drive it positive and the frequencies spread apart, swelling the count of upper partials. Velocity, via the MIDI tab slider, can also drive Inharm. Bear in mind the Pipe and Tube resonators ignore this parameter.

Found only on the Pipe resonator, Opening interpolates between a closed and an open pipe. Set to 0%, one side stays sealed; set to 100%, both ends are open. Velocity on the MIDI tab can drive this parameter too.

Where along the resonator the object gets struck or otherwise set in motion is governed by the Hit slider. Set to 0%, the strike lands dead center. Larger settings shift the strike point toward the edge. Raising the Rnd slider can also scatter the Hit position randomly. Bear in mind the Pipe and Tube resonators ignore this parameter.

How far MIDI Note Off messages silence the resonance is governed by Note Off. Set to 0%, Note Offs go unheeded and decay time follows only the Decay parameter. That mirrors how genuine mallet instruments — marimbas and glockenspiels among them — actually behave. Set to 100%, the resonance cuts off the instant a Note Off arrives, no matter the Decay time.

Where on the left and right resonator the vibrations get picked up is governed by the Pos. L and Pos. R sliders. Set to 0%, the resonance is read at the object’s center. Larger settings shift the pickup point toward the edge. Neither applies to the Pipe or Tube resonators, whose reading is always taken at the midpoint of their permanently open end.
