# Minigame Practice — Cosmetics

Free, public manifest for the custom cosmetics feature in
[Minigame-Practice Client](https://github.com/matheorodriguez).
No account or paid service involved — this is just a JSON file and some PNGs
served over HTTPS via raw.githubusercontent.com.

## Format

`cosmetics.json` maps a Minecraft account UUID (with dashes) to a cosmetic
entry:

```json
{
  "cosmetics": {
    "11111111-2222-3333-4444-555555555555": {
      "cape": "https://raw.githubusercontent.com/<you>/<repo>/main/capes/me.png"
    }
  }
}
```

`cape` must point at a standard Minecraft cape texture (64x32, or 64x64 for
the newer double-tall layout).

The mod polls this file every 5 minutes — edit it and push, no rebuild
needed for anyone already running the mod.
