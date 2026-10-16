# Electric Hammer Fork And Pickup Overview

Open when you need guidance on Electric Hammer Fork And Pickup Overview in Ableton Live.

Context: [Electric](drift-drums-electric-and-external-routes.md#305-electric).

<a id="source-3051-architecture-and-interface"></a>
### 30.5.1 Architecture and Interface

The workings of the electric piano are in fact fairly straightforward. Striking a key on the keyboard sets off a hammer that strikes a fork. A magnetic coil pickup then amplifies that fork's sound and routes it to the output, much as happens with an electric guitar. Two pieces make up the fork, named the tine bar and tone bar. The hammer strikes the fork at the tine bar, whereas the tone bar acts as a tuned metal resonator, dimensioned to yield the right pitch. After the fork starts up, it keeps ringing by itself for quite a while. Releasing the key, however, brings a damper against the fork and silences it sooner.

The Electric interface splits into four primary sections: Hammer, Fork, Damper/Pickup, holding parameters tied to the instrument's tone and sound; plus the Global section, holding parameters that govern overall behavior and performance, including pitch bend and polyphony.

Clicking an individual section opens up every parameter it holds, or you can click the Hammer, Fork, or Damper/Pickup icons to flip among those sections.

Electric’s Hammer, Fork, and Damper/Pickup Icons.

<a id="source-3052-hammer-section"></a>
### 30.5.2 Hammer Section

Electric’s Hammer Section.

The Hammer section holds the parameters that concern the hammer's own physical properties, along with how your playing influences it.

The Stiffness knob sets how hard the hammer's striking surface is. Higher figures emulate a firmer surface, giving a brighter sound, while lower figures give a softer surface and a mellower sound. Velocity and note pitch can also shape Stiffness by way of the Vel and Key sliders located in the display's lower half.

The Noise knob sets the level of impact noise produced as the hammer strikes the fork. Inside the Noise section in the display's lower half, the Pitch slider sets the center frequency of the noise pitch, and the Decay slider sets how long the noise needs to die away to silence. The Key slider sets the degree to which note pitch governs the noise volume.

The Force section sets how forceful the hammer's strike on the fork is. Low Amount figures emulate a gentle strike, while high figures give a forceful strike. Velocity and note pitch can also shape Force through the Vel and Key sliders.

<a id="source-3053-fork-section"></a>
### 30.5.3 Fork Section

Electric’s Fork Section.

The Fork section carries knobs for the Tine and Tone parameters alike, which form the core of Electric's sound-producing mechanism.

Tine governs the part of the fork that the hammer strikes directly.

The Color slider governs the relative loudness of the high and low partials within the tine's spectrum. Low figures yield lower harmonics, and higher figures yield higher harmonics.

The Decay knob sets how long the tine's sound takes to fade away while a note remains held. Note pitch can modulate the tine's volume level by way of the Key slider.

Tone governs the fork's secondary resonance.

The Release slider covers both Tine and Tone, governing how long the fork's sound takes to decay once a key releases. The Decay parameter behaves just as it does within the Tine subsection.

<a id="source-3054-damperpickup-section"></a>
### 30.5.4 Damper/Pickup Section

Electric’s Damper/Pickup Section.
