# Looper Feedback Routing

Open when you need guidance on Looper Feedback Routing in Ableton Live.

Context: [Looper](reverb-limiter-looper-multiband-routes.md#2825-looper).

<a id="source-28251-feedback-routing"></a>
### 28.25.1 Feedback Routing

For [internal routing](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#internal-routings) to other tracks, Looper can serve as both a source and a destination. With this you could, for instance, build Looper overdubs that keep cycling back through the devices on another track. Here’s how to wire it up:

1. Insert Looper on a track.
2. Record at least one pass of material into Looper.
3. Create another audio track.
4. Set the new track’s upper Audio From and Audio To choosers to the track that holds the Looper.
5. Set the new track’s lower Audio From and Audio To choosers to ”Insert-Looper.”
6. Flip the new track’s Monitoring to ”In.”
7. Drop further effects devices into that new track’s device chain.
8. Put Looper into Overdub mode.

From here, Looper’s signal travels out through the other track’s device chain and loops back into Looper itself, so each pass piles on more heavily processed overdub layers.
