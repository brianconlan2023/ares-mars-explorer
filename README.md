# ARES · Mars Explorer

A 3D Mars you can spin, zoom into and drive on. Part of the space explorer collection, alongside LUNA (the Moon) and TERRA (Earth).

## What's in it

- **Mars as it is right now.** An 8K colour map with relief from NASA's MOLA elevation data. The planet's position and spin follow NASA's Mars24 formulas and the IAU orientation model.
- **Live numbers.** Mars time, the Mars Sol Date, the season, the distance from Earth, the signal delay, Perseverance's sol count and the next launch window.
- **Phobos, Deimos, the Sun and Earth** in the sky around it.
- **17 places to explore,** including Jezero, Olympus Mons, Valles Marineris and Gale.
- **Drive a rover in Jezero.** It has six-wheel rocker-bogie suspension, tracks and dust, and a battery that charges in sunlight. Day and night follow real Jezero local time, and the sunsets are blue.
- **New Jezero.** A 15-building human base, shown as a vision of the future. Press *Manifest* to watch it grow from first landing to city.
- **Learn tabs** on water, orbits, the surface, exploration and living on Mars.

## Controls

- **Phone:** drag to spin, pinch to zoom; when driving, use the on-screen joystick.
- **Laptop:** drag and scroll; when driving, use W A S D or the arrow keys.

## Run locally

```
npx serve site
```

## Deploy

The site deploys to Cloudflare Workers as static assets (`wrangler.jsonc`). Workers Builds is connected to this repo, so every push to `main` goes live. To deploy by hand, run `npx wrangler deploy`.

## Credits

- Mars colour map: Solar System Scope (CC BY 4.0).
- Elevation: NASA / JPL / GSFC MOLA.
- Ephemeris: JPL approximate Keplerian elements and NASA GISS Mars24.
- Built with three.js.

The Jezero terrain is procedural, modelled on the crater's layout rather than taken from survey data. The rover sounds are recreations, not the original recordings.
