# surf-zones
~~zero-eight-seven if it was good~~

Collection of zones and configs for [Shavit-Surf-Timer](https://github.com/bhopppp/Shavit-Surf-Timer).
Attempts to mimic KSF's zoning and stripper files as best as possible.

## Usage
(do the following once)
- In `cfg/sourcemod/plugin.shavit-zones.cfg` set `shavit_zones_usesql` to `0`
- In `cfg/sourcemod/plugin.shavit-zones-json.cfg` set `shavit_zones_json_url` to `https://wrldspawn.github.io/surf-zones/z/{map}.json`

(do the following regularly)
- Copy `addons/stripper`
- Copy `addons/sourcemod/configs/shavit-mapfixes.cfg`

## Extras
`cfg` folder exists as a lazy copy-paste for the first steps.

`addons/sourcemod/config/shavit-styles.cfg`
- Removes styles that aren't relevant to surf
- Sets `force_hsw` to `2` (surf variant) in half sideways
- Disables autobhop (mimics KSF but also needed for zoning)

## TODO
(last updated 2025/03/04)

- Tier 1: 12/69
  - surf_aircontrol_ksf: b1 impossible as shared triggers with main
	  - needs targetname differentiation for tracks
	- surf_akai_final: figure out how to fix cp1 teleport velocity
  - surf_awp_sk337_v3: needs a lot of stripper work and zones
	- surf_beyond: test granis' teleport fix stripper config
- Tier 2: 0/165
  - surf_progress_fix: figure out how the linear route will work
  - surf_seaworld_fix: crashes after 2025/02/18 update
- Tier 3: 0/254
- Tier 4: 0/210
- Tier 5: 0/97
- Tier 6: 0/47
- Tier 7: 0/28
  - surf_gigapede: b3 and b6 crash after 2025/02/18 update
- Tier 8: 0/5

### Timer
These are just nice to haves and theres no guarantee I myself will implement them personally.

- zones: optional targetname differentiation for tracks
- zones-json: create file if not existing when calling editmi
- zones-json: remove `possible_on_*`, maybe add actual metadata (authors, creation date)
- zones: custom zone names for bonus credits or maps like classics, progress
