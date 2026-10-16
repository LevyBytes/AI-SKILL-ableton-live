# Audio Testing And Neutrality

Open when you need guidance on Audio Testing And Neutrality in Ableton Live.

Context: [Audio Fact Sheet](audio-fact-sheet.md#38-audio-fact-sheet).

<a id="source-381-testing-and-methodology"></a>
### 38.1 Testing and Methodology

At the time of writing, each Live build runs through an extensive battery of automated checks spanning the full range of Live‘s capabilities. Every new feature brings new checks along with it, and no update ships unless it clears the entire suite.

<a id="source-382-neutral-operations"></a>
### 38.2 Neutral Operations

We call any Live procedure that produces zero alteration in audio quality a _neutral operation_. Relying on these functions guarantees that the signal stays intact. Use a neutral operation on material captured into Live and the result matches the signal exactly as it stood right after analog-to-digital conversion. Use one on files brought into Live and what you get is bit-identical to the versions sitting on disk. Use one while exporting from Live and the rendered file lands at quality no worse than what reached your ears during playback.

Treat the catalog of neutral operations that follows mainly as a theoretical reference. Each entry truly is neutral on its own, yet keep in mind that in practice it nearly always sits inside a chain that also includes non-neutral steps. Take an effects device, for instance: passing a signal through it is non-neutral. Whatever neutral operations come afterward will therefore still hand you audio that has been changed in some respect. Strictly speaking, even nudging the gain counts as non-neutral.

Neutral operations include:
