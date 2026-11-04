# The Warren — a CosyWorld worldpack

A patient burrow beneath Black pond, reached through a crack in the stone.
Whatever the surface discards drifts down there, and the residents keep it:
memory-spores on cool shelves, small refusals recorded as soft chalk marks.
Nothing down there is thrown away twice.

This repository is a **third-party worldpack** for the CosyWorld card table,
published through the worldpack store. It is the reference plugin: the pack
lives here, in its own repo, and reaches the game through the store's
publish-and-pin pipeline rather than as in-tree content.

## Layout

- `card-world.json` — the reusable world (places, residents, items, topics)
- `card-bridge.json` — the crossings joining it to the hub (Black pond)
- `worldpack.json` — the manifest: id, revision, engine contract, contents
- `assets/` — backdrops, portraits and item art (opaque backdrops 1024×576,
  transparent cutouts)
- `PROVENANCE.md` — the generation prompt for every art asset

## The world

**Places:** the Threshold (burrow mouth), the Spore Shelf (kept memory), the
Ledger Nook (kept refusals).

**Residents:** the Hissling, a patient coil of a snake that hatched itself,
keeps the Threshold; the Sifter turns every spore jar a quarter-turn a day so
memories fade evenly — tending, not rescuing.

**Bridge:** the crack beneath Black pond is always open. The way back is the
same crack, climbed slowly.

## Install

Add to the store index (`v2/worldpacks/store.json` in cenetex/cosyworld)
with a pinned commit and content hash; the store build fetches, validates and
vendors the pack. See the store docs in the main repository.
