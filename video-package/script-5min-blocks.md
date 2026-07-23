# 5-Minute Production Script — "A Plane Ran Out of Fuel at 41,000 Feet"

**Pipeline:** Higgsfield `video-explainer` workflow · 30 blocks × 10s = 5:00 exactly
**Video model:** `seedance_2_0` · `mode: std` · `resolution: 1080p` · `duration: 10` · aspect 16:9
**Voice model:** `seed_audio` (one voice, 30 takes — voice picked by user from `list_voices`)
**Character mode:** faceless (no recurring mascot, no on-screen faces as focus)
**Style:** Bright Side–type flat 2D vector edutainment cartoon (style key attached to every clip)

**STYLE tokens (used in every prompt):** flat 2D vector cartoon, bright edutainment style, bold clean outlines, saturated cheerful palette, simple rounded shapes, smooth gradient skies, minimal texture, non-photorealistic, no live-action, no realism

---

## Narration blocks (Phase 2) — one line per 10s block, ~20–24 words each

```
Block 1
You're forty one thousand feet over Canada in a brand new Boeing seven sixty seven, when suddenly, both engines go completely silent.

Block 2
Your one hundred thirty two ton airliner has just become the world's heaviest glider, and the nearest airport is too far away.

Block 3
But what the captain does next has never been attempted in a commercial jet, and it will save every single life on board.

Block 4
It's July twenty third, nineteen eighty three. Air Canada Flight one forty three is preparing to fly from Montreal to Edmonton.

Block 5
The plane is so new it still has that new plane smell, but there's one problem. The fuel gauges aren't working.

Block 6
No big deal, everyone thinks. The crew will simply measure the tanks by hand, and calculate the fuel by weight.

Block 7
Except Canada is switching from the imperial system to metric, and this jet is the very first one calculated in kilograms.

Block 8
The flight needs twenty two thousand three hundred kilograms of fuel. The ground crew does the math using the number for pounds.

Block 9
The paperwork looks perfect. But Flight one forty three takes off with roughly half the fuel it needs, and nobody has any idea.

Block 10
For the first hour, everything is textbook. Sixty one passengers, eight crew members, and smooth summer skies over Ontario.

Block 11
Then, a warning chime nobody has ever heard before. Low fuel pressure in the left tank. Must be a faulty pump, they think.

Block 12
They decide to divert to Winnipeg, just to be safe. Minutes later, another chime. Now it's the right tank too.

Block 13
Then the left engine flames out completely. And soon after, a long loud bong fills the cockpit. Both engines are gone.

Block 14
Total power loss at forty one thousand feet. The fancy computer screens go dark, leaving just a few tiny backup dials.

Block 15
Here's something most people don't know. Without engines, the plane loses the hydraulic muscles that move its control surfaces.

Block 16
Luckily, the seven sixty seven hides a secret gadget. A little propeller pops from the belly and turns wind into emergency power.

Block 17
So a tiny windmill is now helping fly a giant jet. But a windmill can't restart engines, and Winnipeg is sixty five miles away.

Block 18
The plane is falling twenty feet every single second. The crew runs the numbers again and again. They will not make it.

Block 19
But captain Bob Pearson has an unusual weekend hobby. He flies gliders. And that hobby is about to save sixty nine lives.

Block 20
While Pearson glides the jet, first officer Maurice Quintal remembers an old air force base nearby, a place called Gimli.

Block 21
What Quintal doesn't know is that Gimli is no longer an air base. Half of it has been turned into a racetrack.

Block 22
And on this beautiful summer Saturday, it's packed with race cars, campers, and families, right beside the old runway.

Block 23
As they line up, Pearson realizes they're coming in too high, and with no engines, you only get one shot at landing.

Block 24
So he pulls a move straight from his glider toolbox called a sideslip, tilting the huge airliner sideways to drop altitude fast.

Block 25
Passengers later said they could see the faces of people on the ground. At the very last moment, Pearson straightens out.

Block 26
The main wheels slam down at about one hundred seventy five knots, but without full power, the nose gear never locked in place.

Block 27
The nose collapses and grinds down the strip in a shower of sparks, which actually helps slow the giant glider down.

Block 28
The plane shrieks, slows, and stops, right before the crowds. All sixty nine people on board walk away safely.

Block 29
The world calls it the Gimli Glider. The plane is repaired, and incredibly, it keeps flying passengers for twenty five more years.

Block 30
And the best part? The repair van sent to fix it ran out of gas on the way. If you loved this story, hit subscribe.
```

---

## Block video prompts (Phase 3) — Seedance 2.0, style key attached to every clip

Common footer for every block:
- **STYLE REFERENCE:** Match the attached style key EXACTLY — {STYLE tokens above}.
- **NEGATIVE:** color drift, photorealism, 3D render, live-action, lip-sync, talking, voices, narration, captions, on-screen text, letters, numbers, logos, watermark.
- **AUDIO:** ambient only (specified per block) — no voice, no narration, no speech.

```
Block 1
SCENE: A sleek white twin-engine jetliner cruising high above a cartoon cloudscape at golden hour; both engine fan icons flicker and dim to gray.
MOTION: Slow lateral tracking shot alongside the plane; engines visibly spool down; faint speed lines fade away.
AUDIO: soft high-altitude wind, engine hum fading to eerie quiet.

Block 2
SCENE: The same jet seen from below against a huge sky, tilted slightly nose-down, tiny farmland grid far beneath; a distant airport icon sits beyond the horizon line.
MOTION: Slow pull-back revealing the vast empty distance between plane and horizon.
AUDIO: lonely wind, faint creak of airframe.

Block 3
SCENE: Cockpit silhouette from behind: two pilot figures facing a wall of dark instrument panels, one warm light on their determined profiles.
MOTION: Slow push-in toward the pilots; a single dial glows brighter.
AUDIO: quiet tense ambient tone, soft wind.

Block 4
SCENE: Retro 1983 airport scene: the jet parked at a sunny gate, vintage cars and a fuel truck below, maple-leaf-style flag motif on the tail (no lettering).
MOTION: Gentle establishing pan across the tarmac from left to right.
AUDIO: airport ambience, distant jet whine, birds.

Block 5
SCENE: Cockpit close-up of a fuel gauge cluster shown as blank dark screens with a yellow warning sticker shape; a pilot figure taps one gauge.
MOTION: Slow zoom toward the dead gauges; the tap makes them flicker once.
AUDIO: cockpit room tone, two soft taps.

Block 6
SCENE: Ground crew figures under the wing using a long measuring stick in an open fuel port, one holding a clipboard with abstract scribbles (no readable text).
MOTION: Tilt down from wing to the crew; clipboard bobs as figure nods confidently.
AUDIO: outdoor tarmac ambience, metal clink.

Block 7
SCENE: Split-screen motif: left side an old imperial-style scale icon, right side a modern metric cube icon; a cartoon maple leaf flips between them like a coin.
MOTION: The leaf coin spins and lands; the two sides pulse in alternation.
AUDIO: playful ticking, soft whoosh on the flip.

Block 8
SCENE: A big abstract chalkboard with symbolic math: fuel-drop icons multiplied by a wrong-factor symbol; a red wrong-way arrow grows while a fuel truck fills the plane behind it.
MOTION: Camera drifts across the board as the fuel truck hose pulses; the tank level stops at half.
AUDIO: chalk scratches, liquid pouring.

Block 9
SCENE: The jet lifts off into a bright morning sky, but its belly shows a subtle x-ray cutaway: fuel tanks only half full, softly glowing amber.
MOTION: Takeoff tracking shot from runway level, rising with the plane; cutaway glow pulses gently.
AUDIO: muffled takeoff roar fading to serene cruise hum.

Block 10
SCENE: Peaceful cabin interior: rows of simple rounded passenger figures reading and dozing, warm sunset light bands sliding across seats.
MOTION: Slow dolly down the aisle toward the cockpit door.
AUDIO: soft cabin hum, gentle rustling.

Block 11
SCENE: Cockpit panel close-up: a single amber warning light blinks over a stylized left fuel tank icon; two pilot silhouettes exchange a glance.
MOTION: Rack focus from pilots to the blinking amber light, then back.
AUDIO: single repeating soft chime, cockpit hum.

Block 12
SCENE: Simple map graphic of Ontario and Manitoba as flat shapes: a dotted flight path bends toward a Winnipeg star icon; a second amber light blossoms on the right side of frame.
MOTION: The dotted line draws itself as the camera follows; the new warning light pulses.
AUDIO: two chimes, low tense drone.

Block 13
SCENE: Exterior of the jet at dusk: the left engine icon sputters with tiny puff shapes and goes dark, then the right follows; the whole plane dims.
MOTION: Slow orbit around the plane as each engine fades; ambient light drops a notch.
AUDIO: engine sputter, then a deep resonant bong, then wind only.

Block 14
SCENE: Cockpit wide shot: rows of glowing screens wink out one by one leaving a black wall with three tiny lit standby dials; pilot silhouettes lean forward.
MOTION: Push-in as screens die, ending framed on the three small dials.
AUDIO: electric power-down whine, wind through airframe.

Block 15
SCENE: Friendly cutaway diagram of the jet: cartoon muscle icons on the wings and tail connected by glowing hydraulic lines that fade to gray.
MOTION: Camera glides along the fading lines from cockpit to tail.
AUDIO: soft schematic blips, ambient hum.

Block 16
SCENE: Belly of the plane pops open and a small cheerful propeller unit drops into the airstream and starts spinning, feeding a glowing line back into the wings.
MOTION: Close tracking on the little propeller as it spins up; glow travels along the line.
AUDIO: wind gust, rising spin whir.

Block 17
SCENE: Wide shot: the huge silent jet gliding, the tiny spinning propeller glinting beneath it; far ahead a Winnipeg star icon sits beyond a receding horizon.
MOTION: Long slow glide forward; the star icon slips further away as the plane sinks.
AUDIO: steady wind, faint whir.

Block 18
SCENE: Altitude concept: a big vertical gauge beside the gliding plane ticks steadily downward; two pilot silhouettes hunched over a paper chart with dividers.
MOTION: Split framing — gauge dropping on the left, pencil moving on chart at right.
AUDIO: pencil scratches, slow ticking, wind.

Block 19
SCENE: Warm flashback vignette: a small white glider soaring over green cartoon hills, a lone pilot figure at peace; soft round clouds.
MOTION: Graceful banking arc following the glider through the hills.
AUDIO: gentle breeze, distant birds.

Block 20
SCENE: The first officer silhouette points at a map; a memory bubble shows a young airman figure before hangars at an airbase marked with a flag shape (no text).
MOTION: Camera pushes from cockpit into the memory bubble.
AUDIO: cockpit hum, soft nostalgic tone.

Block 21
SCENE: The airbase transforms: hangars fade, half the runway peels into a looping racetrack with tiny race cars and bright flags.
MOTION: Overhead top-down view as the transformation animates across the frame.
AUDIO: distant race car buzz rising.

Block 22
SCENE: Festive ground scene: campers, tents, families of simple rounded figures, kids on bikes, race cars lined along the strip in summer light.
MOTION: Slow pan across the happy crowd toward the long gray strip.
AUDIO: crowd chatter, race engines, cheerful ambience.

Block 23
SCENE: Cockpit POV through the windshield: the strip visible far below but the horizon sits too low — the plane is clearly too high; approach cone overlay glows red.
MOTION: Subtle nose-down drift; the red cone pulses once.
AUDIO: rushing wind, tense low drone.

Block 24
SCENE: The huge jet banks into a dramatic sideslip: wings crossed at an angle, body sliding diagonally, altitude streaks trailing upward.
MOTION: Dynamic three-quarter tracking as the plane crabs sideways and drops fast.
AUDIO: roaring crosswind, airframe groan.

Block 25
SCENE: Ground-level shot: upturned round faces of spectators as the giant silent shadow sweeps over them; the jet's wings level out at the last second.
MOTION: Shadow slides across the crowd; tilt up to the plane snapping level.
AUDIO: wind blast, gasps as ambient murmur.

Block 26
SCENE: Touchdown: main wheels smack the strip with smoke puffs; below the nose, a landing-gear icon flashes amber, unlocked.
MOTION: Low trackside shot racing alongside the speeding jet.
AUDIO: tire screech, rumble, wind.

Block 27
SCENE: The nose dips and grinds along the asphalt, a bright fan of cartoon sparks spraying as the plane plows forward.
MOTION: Sparks light the frame as the camera decelerates with the plane.
AUDIO: metal grinding, hiss, rumble fading.

Block 28
SCENE: The jet at rest, nose down like a bowing giant; evacuation slides deploy and rounded figures slide down onto the strip near the distant crowd.
MOTION: Slow rising crane shot revealing plane, slides, and safe crowd in one frame.
AUDIO: slide whoosh, relieved crowd murmur.

Block 29
SCENE: Triumphant montage: the repaired jet gleaming in flight over a timeline ribbon of rising suns from 1983 toward 2008 (abstract sun icons, no numerals).
MOTION: The plane flies along the ribbon as suns pop up behind it.
AUDIO: uplifting ambient swell, jet hum.

Block 30
SCENE: Comedy beat: a tiny repair van sputters to a stop on an empty cartoon highway with a fuel-drop icon flashing above it; the jet's silhouette soars overhead.
MOTION: Van bounces to a halt; slow tilt up to the plane passing above.
AUDIO: engine sputter, comedic boing, soft wind.
```

---

## Generation parameters checklist

| Step | Tool | Settings |
|---|---|---|
| Style key | `generate_image` / `nano_banana_pro` | 16:9, abstract Bright Side–style swatch, non-photoreal |
| Clips ×30 | `generate_video` / `seedance_2_0` | duration 10 · resolution 1080p · mode std · style key as `image_references` · native ambient audio ON, voices banned in NEGATIVE |
| Voice ×30 | `generate_audio` / `seed_audio` | one user-picked voice_id/voice_type reused on all 30 takes, each ≤9.5s |
| Assembly | `explainer_video` | width 1920 × height 1080, blocks 1→30 in order, clip N + voice take N |
