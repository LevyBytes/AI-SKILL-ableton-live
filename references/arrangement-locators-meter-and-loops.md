# Arrangement Locators Meter And Loops

Open when you need guidance on Arrangement Locators Meter And Loops in Ableton Live.

Context: [Arrangement View](arrangement-view.md#6-arrangement-view).

<a id="source-64-launching-the-arrangement-with-locators"></a>
### 6.4 Launching the Arrangement with Locators

For several playback-trigger spots throughout the Arrangement, drop launchable locators into the scrub area.

Use Locators to Launch Playback in the Arrangement.

With the Set Locator button you can place locators anywhere in the Arrangement on the fly, whether playing back or recording. Each locator is quantized to the global launch quantization value chosen in the Control Bar.

The Set Locator Button.

Pressing the Set Locator button when the transport is idle drops a locator at the insert marker spot, or at where the time selection begins. Locators can likewise be placed through the Add Locator entry in the scrub area’s context menu or by way of the Create menu.

Keep in mind that once locators exist in the Arrangement, the Set Locator button switches to the Delete Locator button for whichever locators are selected.

Reaching a locator is a matter of clicking it or pressing the Previous and Next Locator buttons sitting beneath the Set button. Once you pass the Arrangement’s first or last locator, those Previous and Next Locator buttons carry you to the Arrangement start or end accordingly.

The Previous and Next Locator Buttons.

[MIDI/key mapping](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) can also fire locators. With the transport halted, a double-click on a locator selects it and sets playback rolling from there.

A selected locator can be relocated by dragging it or pressing the arrow keys. Renaming selected locators happens through the Rename entry in the Edit menu or the Ctrl+R (Win) / Cmd+R (Mac) shortcut. You may also attach your own info text notes to locators via the Edit Info Text entry in the Edit menu or the locator’s context menu. Removing a locator is done with the Delete key, the Delete Locator entry under the Create menu, or the Delete Locator button.

A locator’s context menu carries the Loop to Next Locator command, a fast route to [looping playback](https://www.ableton.com/en/live-manual/12/arrangement-view/#the-arrangement-loop) across two locators. The Set Song Start Time Here command overrides the standard “playback starts at selection“ behavior: with it checked, playback fires from the locator rather than the selection.

<a id="source-65-time-signature-changes"></a>
### 6.5 Time Signature Changes

By means of time signature markers, Live’s time signature is adjustable at any spot along the Arrangement. Dropping a marker at the present insert marker position is done with the Insert Time Signature Change command from the Create menu or the scrub area’s context menu.

A marker accepts any time signature whose numerator is one or two digits and whose denominator is 1, 2, 4, 8 or 16. Those two numbers need a separator between them — a slash, comma, period, or however many spaces.

Time signature values can additionally be typed or nudged through the Time Signature Numerator and Denominator fields in the Control Bar. Doing so alters the time signature at the present play spot, and functions whether the transport is halted or rolling.

Whenever the Arrangement holds time signature changes, an automation LED shows up in the upper left corner of the time signature fields.

The Time Signature Fields.

You will find time signature markers sitting right under the beat-time ruler. Bear in mind this marker strip stays hidden when a Set carries no meter changes.

Time Signature Changes.

Moving time signature markers is done with the mouse or the left and right arrow keys. To edit the values of selected markers, reach for the Edit Time Signature command — found under the Edit menu, inside the scrub area’s context menu, or bound to the Ctrl+R (Win) / Cmd+R (Mac) shortcut. Removing a time signature marker calls for the Delete key or the Delete command in the Edit menu.

Time signature markers carry no quantization; you may drop them anywhere along the timeline, with their placement bounded solely by the [editing grid](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid). So meter changes can land in “impossible“ spots — for instance, ahead of the prior measure’s close. That produces a _fragmentary bar_, shown in the scrub area as a crosshatched patch. Live will gladly leave such partial measures untouched, yet should you want your Set to obey music theory, the context menu offers options for “correcting“ those incomplete bars.

A Fragmentary Bar and its Context Menu Options.

_Delete Fragmentary Bar Time_ strips the fragmentary bar’s span out of the Arrangement, drawing whatever audio or MIDI clips flank the removed stretch nearer one another along the timeline. The following time signature marker then lands on the barline you would expect.

_Complete Fragmentary Bar_ adds time at the fragmentary bar’s front, rounding it out to full. The following time signature marker then lands on the barline you would expect.

Do bear in mind that each of these options touches _all_ tracks — removing and adding time alters how long the whole Arrangement runs.

Bringing a [MIDI file](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#midi-files) into the Arrangement offers you the choice to pull in whatever time signature data was stored alongside it. Take that option and Live drops time signature markers into all the right spots on its own. This makes handling intricate music built in other sequencer or notation programs quite painless.

<a id="source-66-the-arrangement-loop"></a>
### 6.6 The Arrangement Loop

For looping a stretch of the Arrangement over and over, switch on the _Arrangement Loop_ with its toggle in the Control Bar.

The Arrangement Loop Toggle in the Control Bar.

With no clip(s) or time selected, the loop brace stretches over the whole Arrangement. Its length is settable by number through the _Loop Start_ and _Loop Length_ fields in the Control Bar, which fix the loop’s starting point and its duration respectively.

The Loop Start Fields (Left) and the Loop Length Fields (Right).

The Edit menu’s Loop Selection command switches on the Arrangement loop and snaps the loop brace to the active time selection. Its matching shortcut, Ctrl+L (Win) / Cmd+L (Mac), will also flip the Arrangement loop on or off whenever a clip or time is selected.

The Arrangement’s Loop Brace.

These keys and commands adjust the loop brace:

- The left and right arrow keys inch the loop brace one way or the other according to the present [grid settings](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid).
- The up and down arrow keys move the loop brace sideways in increments matching the loop brace length.
- Ctrl (Win) / Cmd (Mac) plus the left and right arrow keys trims or extends the loop by the present grid settings.
- Ctrl (Win) / Cmd (Mac) plus the up and down arrow keys doubles or halves the loop length.

Dragging the loop brace works too: pull on its left or right edge to move the loop’s start/end points, or drag the brace bar sideways to reposition the loop while keeping its length the same.

So that playback fires from the loop brace’s start, head into the brace’s context menu and enable Set Song Start Time Here there. Doing so overrides the standard behavior of starting playback at the insert marker or the live time selection.
