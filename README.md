# Black & White FiveM Speedometer

Custom black & white analog speedometer for FiveM.

## Features

- Analog speedometer 0–180 KM/H
- RPM display
- Fuel display
- Vehicle health / HP
- Gear display
- Engine indicator
- High-beam indicator
- Left / right indicator
- Seatbelt indicator
- Seatbelt toggle with `B`
- Automatically hides when the player is not driving
- Standalone: no ESX, QBCore, or Qbox required
- Local NUI: no external website is required at runtime

## Install on FiveM

Put this repository/resource into:

```text
resources/[standalone]/blackwhite_speedometer
```

Then add this to `server.cfg`:

```cfg
ensure blackwhite_speedometer
```

Restart the resource or server.

## Important: GitHub is only for storing the resource

FiveM does **not** need a GitHub Pages link to display this speedometer.

The HTML/CSS/JavaScript files run from the FiveM resource itself.

Recommended workflow:

```text
GitHub Repository
       ↓
Download / clone
       ↓
FiveM resources/[standalone]/
       ↓
ensure blackwhite_speedometer
       ↓
Speedometer runs in FiveM
```

## Controls

`B` — Toggle seatbelt.

## Structure

```text
blackwhite_speedometer/
├── fxmanifest.lua
├── client.lua
├── README.md
└── html/
    ├── index.html
    ├── style.css
    └── script.js
```

## Notes

The odometer in this first version is a visual placeholder. It can be upgraded later to save real distance per vehicle/player in a database.

Fuel currently uses the GTA V native vehicle fuel value. If your server uses a custom fuel script, the fuel value can be integrated with that system.

## License

You may modify this resource for your own FiveM server.
