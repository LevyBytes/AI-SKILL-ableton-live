# Working With Video

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 27. Working with Video

Thanks to its adaptable design, Live works beautifully when you need to compose music for a moving picture. Individual video clips can be cropped down to just the portions you care about, and _Warp Markers_ let you line up your score against the footage right inside the Arrangement View. Once that's done, you can [render](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video) the resulting cut together with the soundtrack you've built.

It helps to first get comfortable with the ideas covered in the [Audio Clips, Tempo, and Warping chapter](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#audio-clips-tempo-and-warping) before you begin.

Should your workflow involve locking Live to outboard video gear, the [chapter on synchronization](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-with-link-tempo-follower-and-midi) is worth a look as well.

### 27.1 Importing Video

Movies saved in Apple's QuickTime format (.mov) can be brought into Live and turned into video clips. Such files show up within Live’s browser, and you load them simply by dragging each one onto the Live Set.

Keep in mind that picture is shown solely for clips that live in the Arrangement View. Any movie dropped into the Session View instead behaves as an ordinary audio clip.

### 27.2 The Appearance of Video in Live

### 27.2.1 Video Clips in the Arrangement View

Apart from the “sprocket holes“ shown along its title bar, a video clip sitting in the Arrangement View is visually indistinguishable from a regular audio clip.

A Video Clip in the Arrangement View.

In nearly every respect, a video clip in the Arrangement View behaves exactly as an audio clip does — you can shorten it, say, by pulling on either its left or right edge. _However_, a handful of edits, once carried out on a video clip, swap it for an audio clip, which of course carries no picture at all. That swap happens purely within Live; the source movie on disk stays untouched. Three operations trigger this behavior: _Consolidate_, _Reverse_ and _Crop_.

### 27.2.2 The Video Window

The Video Window in the Arrangement View.

A detached, floating panel, the Video Window stays parked on top of Live’s primary window at all times. Drag it wherever suits you and it will never end up hidden behind Live. To show or hide it, use the relevant entry in the View menu. Grab its lower-right corner to scale the panel up or down. Because its dimensions and placement aren't tied to any particular Set, those settings come back the next time you load a video. Double-click inside the Video Window to switch to a full-screen view, which you can route to a second display if you prefer. To snap it back to the movie's native dimensions, hold Alt (Win) / Option (Mac) while double-clicking in the Video Window.

#### 27.2.2.1 Movies with Partial Tracks

The QuickTime container permits a movie's sound and picture streams to cover less than its full running time, leaving holes in playback. Wherever the picture drops out, Live’s Video Window goes black; wherever the sound drops out, you simply hear nothing.

### 27.2.3 Clip View

If you write for picture, pay attention to the Tempo Leader control found in Live’s Clip View. The customary setup while scoring puts video clips in the tempo leader role and keeps audio clips acting as tempo followers — and indeed those are the warp defaults Live assigns to Arrangement View clips. Working this way, the Warp Markers you place on a video clip mark the “hit points“ your score has to land on. _Bear in mind that a clip can only take on the tempo leader role once its Warp switch has been turned on_.

Setting a Video Clip as Tempo Leader.

As the [Audio Clips, Tempo, and Warping chapter](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#audio-clips-tempo-and-warping) explains, you may switch on the Tempo Leader option for as many warped Arrangement clips as you wish, yet the genuine leader is always whichever lowest, currently sounding clip holds that flag.

A side effect is that a video clip which isn't acting as the leader can still end up warped, and the Video Window will then show that warped picture.

#### 27.2.3.1 Warp Markers

As you drag a Warp Marker that sits on a video clip, the Video Window keeps pace by displaying the matching frame, making it simple to line any moment of your score up with any moment of the footage.

Because Live surfaces whatever QuickTime markers are baked into a movie file, those markers serve as handy on-screen reference points while you place your Warp Markers.

### 27.3 Matching Sound to Video

Getting going with video in Live is only a short procedure. Consider a typical case — fitting a musical passage to the cuts or hit points within a video:

1. Confirm that Live is showing the Arrangement View. On a one-screen setup, pressing the Tab key on your keyboard flips back and forth between the Session View and Arrangement View.
2. Pull a QuickTime movie out of Live’s browser and release it onto an audio track within the Arrangement View. At that point the Video Window opens up and renders the picture portion of the file. Recall that this window can be relocated anywhere on screen that suits you.
3. With the video clip in place, bring an audio clip into the Arrangement View’s drop area; Live spins up a fresh track to hold it. Expand each track to reveal what's inside by clicking the controls positioned beside their names.
4. Give the video clip’s title bar a double-click to open it in the Clip View. Within the Audio tab/panel, verify that the Warp button is switched on. Any warped clip in the Arrangement View may serve as either tempo leader or follower; here we set the Leader/Follower switch to Leader, so that every other clip in the Live Set conforms to the video clip’s tempo — in other words, its standard playback speed.
5. At this stage, drop Warp Markers onto the video clip and nudge them however you see fit. Where each of the Warp Markers sits establishes the sync anchors tying the music to the picture. Watch the video clip’s waveform in the Arrangement View redraw itself to mirror every adjustment as you go.
6. Should you wish to concentrate on one particular passage of the piece, switch on the [Arrangement Loop](https://www.ableton.com/en/live-manual/12/arrangement-view/#the-arrangement-loop).
7. Once everything's set, pick the Export Audio/Video command out of Live’s File menu. Your whole mix is bounced down and written out as one audio file, and the same command lets you write out your video file too.

### 27.4 Video Trimming Tricks

It's typical for a composer to be handed footage that opens with several seconds of empty space ahead of where the “real“ action kicks off. That pre-roll (“two-beep“) gives the mixing engineer a sync anchor, and they count on the composer's audio files carrying an identical pre-roll. During the writing stage, though, this lead-in just gets underfoot — you'd rather have the on-screen action begin at song time 1.1.1 and SMPTE time 00:00:00:00. Trimming the video clips, as described below, makes that possible.

1. To begin, place a movie file right at the Arrangement's opening point (1.1.1).
   A Video Clip at the Start of the Arrangement.
1. After that, double-click the video clip’s title bar so its contents open in the Clip View. From there, pull the Start Marker rightward until the video clip begins exactly where the action does.
   Dragging the Start Marker behind the Pre-Roll.
1. With that done, your on-screen action and the score you'll write both line up at 1.1.1 / 00.00.00.00. After the music is finished and you're set to render it out, the pre-roll has to be reinstated:
1. Over in the Arrangement View, grab everything (Edit menu/Select All) and shift the whole composition rightward by a few seconds:
   The Video Clip and the Final Clip of Music.
1. Finally, click the video clip’s title bar so nothing else stays selected, then pull its left edge leftward as far as it goes to bring the pre-roll back into view.
   The Video Clip with Pre-Roll Restored.

Out of the box, the Export Audio/Video command produces sample files that match the length of whatever the Arrangement selection covers; since the video clip remains part of that selection, the resulting sample file runs precisely as long as the source movie did, pre-roll and all.
