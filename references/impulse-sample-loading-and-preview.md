# Impulse Sample Loading And Preview

Open when you need guidance on Impulse Sample Loading And Preview in Ableton Live.

Context: [Impulse](drift-drums-electric-and-external-routes.md#307-impulse).

<a id="source-3071-sample-slots"></a>
### 30.7.1 Sample Slots

<a id="source-live-instrument-reference-part-4"></a>

You can drag samples onto any of Impulse’s sample slots straight from the browser or from the Session and Arrangement Views. As another option, every sample slot carries a Hot-Swap button for [hot-swapping samples](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#hot-swapping-samples). To remove a loaded sample, press the Backspace (Win) or Delete (Mac) key.

Once imported, samples map themselves automatically across your MIDI keyboard, so long as that keyboard is connected and recognized by Live. Pressing C3 fires the leftmost sample, with the remaining samples laid out in sequence across the octave spanning C3 to C4. With the Fold button on, Impulse’s eight slots show up labeled within the [MIDI Editor’s key tracks](https://www.ableton.com/en/live-manual/12/editing-midi/#editing-midi), regardless of whether a particular key track holds any MIDI notes. To shift this mapping away from its default, add a [Pitch](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#pitch) device; to reorder it instead, add a [Scale](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#scale) device.

Every one of the eight samples carries its own dedicated set of parameters, which sit in the region beneath the sample slots and become visible once you click a sample. Changes you make to a sample’s settings register only when the next note arrives — notes already sounding are left untouched. Keep in mind that this same logic governs how Impulse responds to parameter shifts coming from clip envelopes or automation, since those too take hold only as a fresh note begins. Should you instead need changes that evolve while a note sustains, the [Simpler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#simpler) instrument is the better choice.

Among Slot 8’s parameters is a Link button, sitting in the lower left corner, which ties slot 8 to slot 7. With these two slots linked, triggering slot 7 halts slot 8’s playback, and the reverse holds true as well. The intent behind this feature was a particular scenario (though naturally you can apply it elsewhere): emulating how a closed hi-hat cuts off an open one.

Hover the mouse over any slot and controls appear letting you play, solo, mute, or hot-swap it.
