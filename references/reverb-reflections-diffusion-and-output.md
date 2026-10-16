# Reverb Reflections Diffusion And Output

Open when you need guidance on Reverb Reflections Diffusion And Output in Ableton Live.

Context: [Reverb](redux-resonators-reverb-and-roar-routes.md#2832-reverb).

<a id="source-28321-input-filter"></a>
### 28.32.1 Input Filter

Reverb’s Input Filter Section.

First in the chain, the signal meets low and high cut filters whose X-Y controller sets the band’s center frequency on the X-axis and its bandwidth on the Y-axis. You can also operate the filters with the sliders sitting beneath the X-Y controller. When either filter isn’t required, switching it off conserves CPU power.

<a id="source-28322-early-reflections"></a>
### 28.32.2 Early Reflections

Reverb’s Early Reflections Section.

What you hear soonest are these echoes, arriving as the sound rebounds off the room’s walls ahead of the diffused reverberation tail setting in. The way they spread out, and how loud they are, conveys a sense of the room’s character.

Modulation of the early reflections is handled by Spin. Its Amount and Rate sliders govern how much modulation occurs and how fast, respectively. Pushing the Amount higher generally yields a late diffusion response that is more spectrally neutral and less colored. Should the modulation rate climb too high, doppler-style pitch shifting of the source sound creeps in, accompanied by surreal panning artifacts. To save a little CPU, Spin can be switched off via its associated switch.

How prominent the early reflections are, and how much they overlap the diffused sound, is shaped by the Shape control. At lower settings, the reflections fade more gently and the diffused sound arrives earlier, so these two elements overlap more. At higher settings, the reflections fade quicker and the diffused onset comes later. Raising the value can occasionally sharpen the source’s clarity, whereas a lower value tends toward a smoother decay.

<a id="source-28323-diffusion-network"></a>
### 28.32.3 Diffusion Network

Reverb’s Diffusion Network Section.

It is the Diffusion Network that generates the reverberant tail trailing the early reflections.

Frequency-dependent reverberation decay comes from the high and low shelving filters. The decay at high frequencies mirrors how air, walls, and other materials in the room — occupants, carpet, and the like — absorb sound energy. A thinner decay is supplied by the low shelf. Switching either filter off lowers CPU consumption.

Density and coarseness of the diffusion can be further shaped with the Diffusion and Scale parameters, which, when the room is set to an extremely small size, weigh heavily on the coloration the diffusion introduces.

<a id="source-28324-chorus"></a>
### 28.32.4 Chorus

Reverb’s Chorus Section.

A touch of modulation and movement is added to the diffusion by the Chorus section. You can set its modulation Amount and Rate, or switch it off entirely.

<a id="source-28325-global-settings"></a>
### 28.32.5 Global Settings

Reverb’s Global Settings.

How long the device waits, in milliseconds, before the first early reflection begins is governed by Predelay, which pushes the reverberation back in time relative to the input. Part of how large a real room seems comes down to this delay. For natural-sounding material, expect figures somewhere between 1 ms and 25 ms.

When you adjust the Size parameter, the Smooth chooser dictates how that change behaves. Choose None and the Diffusion Network’s delay times jump instantly, which can introduce artifacts as the Size value moves. Choose Slow or Fast and the new delay times settle in across a set interval, giving a smoother transition between values.

How big the room is comes down to the Size parameter. Pushed to its upper limit, a very large size gives the reverb a shifting, diffused delay quality. Pulled to the opposite extreme, a very small value makes it sound highly colored and metallic.

Use the Decay control to set how long the reverb tail takes to fall to 1/1000th (-60 dB) of where it started.

What the Freeze control does is hold the diffuse response of the incoming sound in place; with it on, the reverberation rings on nearly forever. While Freeze is engaged, Flat bypasses both the high and low shelf filters. Leave Flat off and the frozen reverberation will bleed energy from the attenuated bands according to how the high and low shelving filters are set. Cut alters Freeze so the input signal no longer feeds the frozen reverberation; with it off, the input does add to the diffused amplitude.

The width of the output’s stereo image is set by the Stereo control. Turned all the way up to 120 degrees, each ear gets its own reverberant channel fully independent of the other — something real rooms exhibit in their diffusion too. Turned all the way down, the output is summed to mono.

A balance between reverb quality and CPU cost is struck with the Density chooser. Sparse keeps CPU usage to a minimum, whereas High produces the most lavish reverberation.

<a id="source-28326-output"></a>
### 28.32.6 Output

Reverb’s Output Section.

Right at the reverb’s output stage, the Reflect and Diffuse controls let you scale the level of reflections and diffusion, and you can set the effect’s overall Dry/Wet mix here as well.
