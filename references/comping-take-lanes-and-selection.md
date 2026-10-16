# Comping Take Lanes And Selection

Open when you need guidance on Comping Take Lanes And Selection in Ableton Live.

Context: [Comping](bouncing-and-comping-routes.md#21-comping).

<a id="source-211-take-lanes"></a>
### 21.1 Take Lanes

Each audio or MIDI track in the [Arrangement View](https://www.ableton.com/en/live-manual/12/arrangement-view/#arrangement-view) may hold several parallel lanes. A track’s very first lane is the main lane, audible by default. On top of that, a track can carry as many take lanes as you like, though those sound only while [Audition Mode](https://www.ableton.com/en/live-manual/12/comping/#auditioning-take-lanes) is turned on.

A Track’s Main Lane.A Track’s Take Lanes.

Live generates take lanes for you when you're [recording new clips](https://www.ableton.com/en/live-manual/12/comping/#recording-takes) in the Arrangement, and you can additionally [insert them manually](https://www.ableton.com/en/live-manual/12/comping/#inserting-and-managing-take-lanes).

To switch take lanes between shown and hidden, you have two choices: from a track header’s context menu, pick the Show Take Lanes command; otherwise, flip the Show/Hide Take Lanes toggle in a track’s main lane.

The Show/Hide Take Lanes Toggle.

Showing or hiding take lanes is bound to Ctrl+Alt+U (Win) / Cmd+Option+U (Mac).

Pressing the left arrow key moves you from a take lane back to the main lane and, in doing so, folds all the take lanes.

Bear in mind that take lanes stay hidden while [Automation Mode](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation) is active. The Show Take Lanes command and take-lane insertion remain available during Automation Mode, but performing either one leaves the mode and reveals all take lanes.

<a id="source-212-inserting-and-managing-take-lanes"></a>
### 21.2 Inserting and Managing Take Lanes

To add a take lane by hand to one or several selected tracks, choose the Insert Take Lane command from the Create menu. That same command is also available from a track or take lane header’s context menu, or through the shortcut Shift+Alt+T (Win) / Shift+Option+T (Mac). Adding a take lane will additionally unfold any current lanes that aren't yet on display.

It's worth noting that you can likewise build take lanes and drop clips into existing ones through [the Live API with Max for Live](https://docs.cycling74.com/apiref/lom/takelane/).

Duplicating take lanes is done with the Ctrl+D (Win) / Cmd+D (Mac) shortcut, or through the Duplicate command in a take lane header’s context menu.

Removing take lanes happens via the Backspace or Delete key, or through the Delete command in the Edit menu.

To clear every take lane off a track, open a track or take lane header’s context menu and reach for the Delete All Take Lanes command. Meanwhile, the Delete All Unused Take Lanes command clears out any take lanes lacking [recorded material within a comp](https://www.ableton.com/en/live-manual/12/comping/#creating-a-comp) on the track’s main lane.

For vertical resizing of take lanes, two key combos grow or shrink them: Alt++ (Win) / Option++ (Mac) and Alt+- (Win) / Option+- (Mac). A third option holds Alt (Win) / Option (Mac) while you scroll the mouse wheel. Each of these acts on all the selected take lanes at once.

Hovering over a take lane’s edge surfaces resize handles, which likewise let you set the height of one or several selected lanes.

Rearranging take lanes inside their track works by dragging and dropping, or by holding the Ctrl (Win) / Cmd (Mac) modifier and tapping the up or down arrow key.

For renaming take lanes, the Rename command does the job, found either in the Edit menu or in a take lane header’s context menu. Its keyboard shortcut is Ctrl+R (Win) / Cmd+R (Mac). You can rename several take lanes at once, and the Tab and Shift+Tab shortcuts step you between lanes and tracks as you rename.

<a id="source-213-recording-takes"></a>
### 21.3 Recording Takes

As you're [recording new clips](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-into-the-arrangement) in the Arrangement View, Live appends take lanes to [armed audio and MIDI tracks](https://www.ableton.com/en/live-manual/12/recording-new-clips/#arming-record-enabling-tracks) on its own and fills those take lanes with clips.

When you record over clips that are already there, whether through separate passes or by recording inside a [loop](https://www.ableton.com/en/live-manual/12/arrangement-view/#the-arrangement-loop), each pass gains a fresh take lane. Live reuses an existing take lane on its own whenever nothing else sits past the punch-in point.

A track’s most recent recorded clip is always duplicated onto that track’s main lane, ensuring it sounds right away during Set playback.

Keep in mind that recorded clips take on their track’s color by default. If you'd rather, set Live to hand each take its own color by switching the Clip Color toggle to Random in the Theme & Colors Settings.

<a id="source-214-inserting-samples"></a>
### 21.4 Inserting Samples

Samples and MIDI files can be dragged onto take lanes straight from the browser or from File Explorer/Finder. With several samples chosen, hold the Ctrl (Win) / Cmd (Mac) modifier key as you drag so each sample lands on consecutive tracks.

<a id="source-215-auditioning-take-lanes"></a>
### 21.5 Auditioning Take Lanes

To audition a take lane, click the Audition Take Lane button (shown as a speaker icon) within that take lane’s header, or press the T keyboard shortcut.

The Audition Take Lane Button.

Bear in mind that although take lanes belonging to different tracks can be auditioned together, each track allows only one take lane to be auditioned. Where a time selection or a lane header selection spans several take lanes across different tracks, the lane chosen last on each track is the one auditioned.

<a id="source-216-creating-a-comp"></a>
### 21.6 Creating a Comp

Whatever you've selected on take lanes can be sent to the main lane either by hitting the Enter key or through a take lane’s Copy Selection to Main Lane context menu command.

You can swap the clips on a track’s main lane for the next or previous take lane clips: select clip headers or make a time selection inside the main lane or a take lane, then hold Ctrl (Win) / Cmd (Mac) and press the up or down arrow key. When the time selection sits on a take lane, the selection itself advances to the next or previous take as well. Bear in mind that empty take lanes get skipped.

Swapping Part of a Clip for Content Taken from Another Take Lane.

While in Draw Mode, the take lane material you've selected can land on a track’s main lane in a single motion: click, drag, then let go of the mouse. You can also overwrite the clips inside a main-lane time selection by clicking a take lane, which drops that take’s matching portion into the selection.

Whatever clips arrive on a track’s main lane are standalone copies of their take lane counterparts. As a result, you can edit main-lane clips however you wish without touching the original take lane clips, and the reverse holds too. Take lane clips accept the same editing as any other Arrangement View clip: moving, copy/paste, drag/drop, consolidating, cropping, or duplicating. You can also shift take lane clips into Session View clip slots either by copy and paste or by drag and drop.

To avoid clicks where clips meet, head to the Record, Warp & Launch Settings and switch on the Create Fades on Clip Edges option there. With it on, four-millisecond crossfades appear automatically between neighboring clips. You can also build those crossfades by hand: select several clips and press Ctrl+Alt+F (Win) / Cmd+Option+F (Mac).

<a id="source-217-source-highlights"></a>
### 21.7 Source Highlights

Wherever a comp sits in a main lane, the matching source material across its take lanes appears tinted in the track’s color. Take lane material that goes unused shows up in a muted, desaturated version of that same track color. The contrast makes it simpler to spot which recordings feed into the comp. Bear in mind that source highlights appear only when the clips line up in position and properties.

A Comp’s Source Material Highlighted Across a Take Lane.

By dragging a highlight’s edge, you can resize the source highlights on take lanes and thereby shift the split point separating two neighboring parts of a comp.

Drag to Shift the Split Point Between Two Neighboring Parts of a Comp.
