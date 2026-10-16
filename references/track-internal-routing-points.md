# Track Internal Routing Points

Open when you need guidance on Track Internal Routing Points in Ableton Live.

Context: [Internal Routings](routing-and-i-o.md#175-internal-routings).

<a id="source-1751-internal-routing-points"></a>
### 17.5.1 Internal Routing Points

A signal leaves each of Live’s tracks, moves through that track’s device chain, and arrives at the track mixer, where the tracks’ faders may pan it or change its level.

Anytime a track’s Audio From input chooser points at another track (the previous section’s Approach 2), you can tap the incoming signal at one of three spots picked in the Input Channel chooser: _Pre FX, Post FX_ or _Post Mixer_.

Tap Points for Track Routing.

- _Pre FX_ grabs the signal straight off a track before it has reached the track’s device chains (FX) or mixer. Because of that, edits to the tapped track’s devices or mixer leave the tapped signal unchanged. Soloing a track that taps another one Pre FX lets you hear that tapped track.
- _Post FX_ grabs the signal at the end of a track’s device chains (FX) but ahead of its return to the track mixer. Consequently, edits to the tapped track’s devices reshape the tapped signal, whereas edits to its mixer settings do not. Soloing a track that taps another one Post FX lets you hear that tapped track.
- _Post Mixer_ grabs a track’s final output once it has run through its device chains and mixer. Soloing a track that taps another one Post Mixer does _not_ let you hear that tapped track.
