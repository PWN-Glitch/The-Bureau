# The Bureau of Last Resorts

A big red button. Nine escalating measures standing between you and it. A room with a very specific way of handling an emergency.

One file, `index.html`, with no build step, no dependencies and no network calls. Open it and press the button.

## What it is

The Bureau of Last Resorts runs an Emergency Measure System on Sublevel 9, and it has one control left. It is big. It is red. It says DO NOT PRESS.

Everything else on screen is bureaucracy: a masthead, an ON AIR light, a live transcript of what the Bureau is doing about you, and a footer counting the measures released so far. The prose is the joke as much as the button is.

## Run it

Open the file directly:

```
open index.html          # macOS
xdg-open index.html      # Linux
start index.html         # Windows
```

Or serve it on a local port, which is handy if you want to test on a phone:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000.

It deploys as-is to any static host. On GitHub Pages, point the repository at `main` and the root folder.

## What the button does

Each press releases one measure and the Bureau writes it down. The first press makes a noise and shakes the room. After that, roughly in order: the lights go out and get rerouted to the button, gravity is temporarily reconsidered, seven unauthorised duplicate buttons appear, you are asked to fill in Form 27-B for permission to have already pressed it, four thousand rubber ducks are airdropped, the button starts dodging your cursor, the typography escapes containment, local spacetime is adjusted for administrative reasons, and finally the room goes quiet and grey.

The tenth press ends the transmission.

There is also a mug, ten teas, and a sound toggle in the footer. All audio is synthesised with the Web Audio API, so nothing is downloaded and nothing plays until you first click. If the browser asks you to interact before allowing sound, that first press counts.

Keyboard usable and announced by screen readers, honours `prefers-reduced-motion` by dropping the shaking and looping animation, and has breakpoints down to phone width.

<details>
<summary>Spoiler</summary>

It was tea. Pressing the small red button on the last screen pours one of ten cups, chosen at random, which is the only part of the system that has ever worked properly. "Reopen the Bureau" puts everything back.
</details>
