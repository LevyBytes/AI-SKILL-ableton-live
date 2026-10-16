# Spectrum And Tuner

Open when you need guidance on Spectrum And Tuner in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2838-spectrum"></a>
### 28.38 Spectrum

The Spectrum Device.

Spectrum carries out live frequency analysis on the audio arriving at it. Its findings appear as a graph, dB running up the vertical axis and frequency/pitch running across the horizontal. Peak readings stay drawn on the graph until you restart the song. Keep in mind that Spectrum is a measurement tool rather than an audio effect — it leaves the incoming signal untouched.

How many samples get examined per measurement is governed by the Block chooser. Larger settings sharpen accuracy while loading the CPU more heavily.

Channel picks which channel gets analyzed — left, right, or both.

How frequently Spectrum runs an analysis comes from the Refresh slider. Like the Block parameter, it trades accuracy against CPU load. Quicker response brings more accuracy yet leans harder on the CPU.

With the Avg slider you state how many sample blocks get averaged for every display refresh. At a value of one, every block appears on its own. That makes the display far busier, which helps when hunting down the spectrum of brief peaks. Raising the Avg value smooths the refresh, showing the spectrum averaged over time, which lines up better with how our ears truly perceive sound.

The Graph button flips the spectrum between a single interpolated line and separate frequency bins.

Max turns the readout of the running peak amplitude on or off. While Max is active, a click in the display clears the stored maximum amplitude.

Using the Scale X buttons you can swap the frequency display’s scaling among linear, logarithmic, and semitone. Note that logarithmic and semitone share the same scaling and merely change the legending at the display’s top from Hertz to note names. Linear scaling shines when you analyze high frequencies in detail.

Hovering your pointer across Spectrum’s display brings up a box reporting the amplitude, frequency, and note name beneath the cursor. At the lower left of Spectrum’s interface, the Range/Auto button swaps between adjusting the display’s dynamic range by hand or automatically. Under Range, you zoom and scroll the amplitude by moving over the amplitude legending along the display’s left edge — drag up and down to scroll, side to side to zoom. The Range sliders likewise let you fix the lowest and highest amplitude values on view. Under Auto, the display rescales itself in response to the incoming audio level. Note that the Range sliders and zooming go inactive while Auto is engaged.

For a still clearer look, swap where the display sits — the device chain or Live’s main window — by clicking the button on Spectrum’s title bar, or simply double-click inside the display.

<a id="source-2839-tuner"></a>
### 28.39 Tuner

The Tuner Device.

Tuner reads out the arriving monophonic pitch together with how far it sits from the closest semitone. Modeled on traditional guitar tuners, its oversized display reads easily from across a stage and excels at tuning outboard instruments or synthesizers.

Bear in mind that Tuner serves as a measurement tool, not an audio effect – the incoming signal passes through unchanged. It is built to read monophonic pitches and performs best on a tidy, well-defined signal. Polyphonic, noisy, or harmonically dense input can throw off its readings.
