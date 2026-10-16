# Tension String Excitation

Open when you need guidance on Tension String Excitation in Ableton Live.

Context: [String Tab](simpler-and-tension-routes.md#30122-string-tab).

<a id="source-301221-the-exciter-section"></a>
#### 30.12.2.1 The Exciter Section

Tension’s Exciter Section.

<a id="source-301222-exciter-types"></a>
#### 30.12.2.2 Exciter Types

You can sound the modeled string with a range of exciters so as to mimic various instrument types and playing styles.

A switch beside its name turns the Exciter section on or off. While it's off, only contact with its damper can excite the string. Should you deactivate both the Exciter and Damper sections, there's nothing left to start the string vibrating — so if no sound emerges, confirm that at least one of these sections is active.

Four options appear in the Exciter Type chooser - _Bow, Hammer, Hammer (bouncing)_ and _Plectrum_.

_Bow_ — tied to bowed instruments like the violin, viola or cello, this exciter drives the string into continuous oscillation. As the bow hair travels over the string, friction makes the string repeatedly cling to the hair and then release. How frequently that stick-and-slip cycle repeats sets the fundamental pitch. Keep in mind the Damping knob is disabled while the Bow exciter is chosen.

_Hammer_ — this exciter recreates the action of soft hammers or mallets. Hammer simulates a hammer sitting beneath the string that strikes it a single time, then drops away. A piano is one place this kind of mechanism turns up.

_Hammer (bouncing)_ - this exciter resembles _Hammer_, but it instead simulates a hammer positioned over the string and let fall onto it, so it may rebound off the string several times. A hammered dulcimer is one instrument where this playing style appears.

_Plectrum_ — a plectrum, or “pick“, goes with instruments like guitars and harpsichords. Picture it as a slanted object tucked beneath the string that flicks the string into motion.

<a id="source-301223-exciter-parameters"></a>
#### 30.12.2.3 Exciter Parameters

Five parameter knobs sit alongside the Exciter Type chooser. Which Exciter Type you pick determines the first two parameters, while the remaining three stay the same across all types.

_Bow Parameters:_

- The Force knob sets how much pressure the bow exerts on the string. Raising this value gives the tone a more “scratchy“ character.
- The Friction knob sets the degree of friction between the bow and the string. Larger values typically yield a quicker attack.

_Hammer / Hammer (bouncing) Parameters:_

- The Mass knob sets the hammer's mass.
- The Stiffness knob sets how rigid the hammer's striking surface is.

_Plectrum Parameters:_

- The Protrusion knob sets how far the plectrum's surface reaches under the string. Smaller values give a “thinner,“ slighter tone, since less mass drives the string into motion.
- The Stiffness knob sets how rigid the plectrum is.

_Universal Exciter Parameters:_

- The Velocity knob sets how fast the exciter drives the string.
- The Position knob defines where along the string the exciter touches it. At 0% the exciter meets the string at its termination point, and at 50% it strikes the string's midpoint. Once the Fix. Pos switch (covered further below) is on, however, position no longer scales with the string's length.
- The Damping knob sets how much of the exciter's striking energy gets reabsorbed into the exciter. Note: With the _Hammer (bouncing)_ exciter this roughly parallels the Stiffness parameter, except that rather than the rigidity of the hammer's surface it governs the rigidity of the virtual “spring“ linking the hammer to the mass driving it. Raising the Damping value shortens the contact between hammer and string, which usually yields a louder, brighter result.

When you engage the Fix. Pos switch, the contact point stays locked to one spot instead of shifting as the string's length changes. That mirrors a guitar, where the picking spot stays roughly constant no matter which notes you play. With a piano the exciter position is proportional — the hammers typically hit the string near 1/7th of its length — so it's best captured with Fix. Pos switched off.

Lastly, the Vel and Key sliders let you modulate these behaviors according to note velocity and pitch respectively.

Do keep in mind that the parameters in the Exciter section interact tightly to shape how the instrument behaves overall. Some setting combinations can leave you with no sound whatsoever.
