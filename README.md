Dust Shift
A 3D factory housekeeping game from Legends Equipment — designers and builders of industrial central vacuum systems.

Third shift at the plant. Combustible dust is settling faster than the crew can sweep it, and you're the one on the hose. Drag it to a wall drop, plug in, and pull the floor clean. Last ten minutes and the plant makes it to morning.

▶ Play it here: (add your GitHub Pages link once the repo is published)

How to play
Control	Action
W A S D	Walk — you turn as you go, and the wand holds that direction
E	Connect at a drop, and walk back to it to unplug
Hold click / Space	Vacuum
Q	Suck Norris (once earned)
R	FiberLight (once earned)
P	Pause  ·  Esc End shift  ·  M Mute
Suction only runs while you're plugged into a drop, and the hose does not stretch — walk too far and it goes taut. Every pile left on the floor drives the combustible dust level up. Hit 100% and the alarm sounds.

Watch the aisles: lift trucks run four different lanes through the plant and the plant manager's golf cart wanders wherever it likes. Either one will crush your hose and flatten you for ten seconds. At the eight-minute mark, a one-ton bulk bag goes over in the center aisle.

Upgrade cards
Every pound you recover fills the upgrade meter. Fill it and three cards come up — they stack for the rest of the shift.

Card	What it does
Hose Extension	+25 ft of hose per level
Larger Hose	Steps the bore up 1.5 in. → 2.5 in.; more air at the tool
Additional Drop	Two more inlet valves tapped into the main
Horsepower	+90 CFM and +11 in. of lift per level
Dust Dozer	Wide-body floor tool — heavy piles come up 75% faster
Pile Diver	Splitter head: two tools at once, and reaches dust on equipment
FiberLight	24 ft lit carbon pole — clears everything overhead on R
Suck Norris	Twin-barrel handheld: 10× recovery for five seconds on Q
Hose Hounds	Retractable reels — release anywhere and the hose runs itself home
Series 2000 Hose	Crush-resistant; survives being run over
Dust Hazards Analysis	The NFPA 652 study — the dust level climbs 22% slower
Energy Drink	Faster on your feet. Past the third can, your hands know it
Running it
One file, no build step, no dependencies to install. Open index.html in any modern browser, or serve the folder over HTTP.

Three.js is loaded from a CDN at runtime; everything else — the factory, the hose simulation, the soundtrack — is generated in the page.

How it works
The hose is a verlet rope. A second invisible "taut path" solve finds the shortest route from the inlet to your tool around whatever equipment is in the way, and that is what gets measured against the reel — so wrapping the hose around a press genuinely costs you reach.
The factory is a fixed-camera cutaway. Walls and roof trusses between the camera and the operator fade out as you move.
The audio is synthesized live — an upbeat groove in F major that switches to a driving track in D minor when the dust level passes 80%.
About
Every upgrade in this game is a real thing Legends Equipment sells: hose runs, additional drops, larger separators and turbine packages, and the tool kits that go on the end of the hose. Housekeeping is a system, not a chore.
