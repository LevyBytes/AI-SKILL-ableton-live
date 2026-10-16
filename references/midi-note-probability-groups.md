# MIDI Note Probability Groups

Open when you need guidance on MIDI Note Probability Groups in Ableton Live.

Context: [Editing Probabilities](midi-note-operations-routes.md#10513-editing-probabilities).

<a id="source-105131-probability-groups"></a>
#### 10.5.13.1 Probability Groups

On top of giving each note its own probability value, you can hand a single probability value to a whole group of notes, so that either every note in the group plays by that value or just one note from the group sounds at any given moment. The two probability group types on offer are:

_Play All_ — every note plays at the probability value fixed by a probability marker. _Play One_ — at any moment only one note from the group sounds, following the set probability, and which note that is gets picked at random.

To build a note probability group, select the notes you want bundled together and click either the Play All or Play One button on the Clip Content Toolbar, according to which probability group type you mean to make.

Play All and Play One Buttons.

After grouping, the Chance Editor shows the notes a lone probability marker: it sports a diamond handle when the group is a Play All type and a triangle handle when it’s a Play One type. Right-click a group probability marker to switch the probability group type. The Play All or Play One buttons on the Clip Content Toolbar flip the group type just as well.

Beyond those dedicated buttons, a few other routes build note probability groups:

- Reach for the Group Notes (Play All) or Group Notes (Play One) context menu options in the MIDI Note Editor.
- Use the Group Notes (Play All) or Group Notes (Play One) command on the Edit menu.
- Hit the Ctrl+G (Win) / Cmd+G (Mac) keyboard shortcut, which produces a group matching the type of the one you most recently built through either the dedicated buttons or the context menu.

Hover over a note that sits in a group and all of that group’s notes light up. Whenever the selected notes belong to a probability group, the Status Bar reports the group’s type — spelled out plainly if every note shares one group, or flagged with an asterisk when they don’t.

That small triangle in the upper-left corner of notes whose probability falls under 100% always appears once a note joins a probability group, even where the group’s probability stands at 100%.

To pull a note out of a probability group, select it and click the Ungroup button on the Clip Content Toolbar. Folding a note into a different group likewise strips it from its first group automatically. To dismantle a probability group entirely, select all of its notes and then click Ungroup.

The Ungroup Button.

The same thing happens through the Edit menu’s Ungroup Notes command, the Ctrl+Shift+G (Win) / Cmd+Shift+G (Mac) shortcut, or a right-click on a grouped note marker followed by choosing the Ungroup Notes option. Once notes are ungrouped, the Chance Editor goes back to showing a separate probability marker for each note.
