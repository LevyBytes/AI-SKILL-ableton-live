# External Audio Mono And Stereo Routing

Open when you need guidance on External Audio Mono And Stereo Routing in Ableton Live.

Context: [External Audio In/Out](routing-and-i-o.md#172-external-audio-inout).

<a id="source-1721-monostereo-conversions"></a>
### 17.2.1 Mono/Stereo Conversions

Select a mono signal as the input of an audio track and the track captures mono samples; pick anything else and it captures stereo samples. Regardless, the signals flowing through the track’s device chain remain stereo, whether the track’s input is mono or the track is playing mono samples.

Conversion from mono to stereo is nothing more than feeding the same signal to both the left and right channels. Conversely, when a track feeds a mono output, the left and right signals get summed and then trimmed by 6 dB to keep clipping at bay.
