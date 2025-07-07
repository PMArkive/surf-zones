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
- Requires [shavit-style-backwards](https://github.com/PMArkive/random-shavit-bhoptimer-stuff/blob/main/shavit-style-backwards.sp) for backwards style

## TODO
(last updated 2025/07/07)

- Tier 1: 48/72
  - surf_1998: s3 skip lasers
  - surf_4am: s4 easy skip fix, s7 key skip fix
  - surf_aircontrol_ksf: b1 impossible as shared triggers with main
	  - needs targetname differentiation for tracks
	- surf_akai_final: figure out how to fix cp1 teleport velocity
  - surf_awp_sk337_v3: needs a lot of stripper work and zones
  - surf_boreas: ksf has different checkpoints than triggers?
  - surf_demise: b1 trigger weirdness
  - surf_derpis_ksf: lasers
  - surf_egypt2: lasers
  - surf_funhouse_v1: bunch of stripper work
  - surf_mesa_fixed: checkpoint 1 isnt exact on both sides but shrug
- Tier 2: 0/166
  - surf_progress_fix: figure out how the linear route will work
  - surf_seaworld_fix: remove spherical brushes
- Tier 3: 0/255
  - surf_s_t_a_t_i_o_n: remove spherical brushes, laser teleport
- Tier 4: 0/213
- Tier 5: 0/100
- Tier 6: 0/50
- Tier 7: 0/29
  - surf_gigapede: remove spherical brushes
- Tier 8: 0/6

### Timer
These are just nice to haves and theres no guarantee I myself will implement them personally.

- zones: optional targetname differentiation for tracks
- zones-json: create file if not existing when calling editmi
- zones-json: remove `possible_on_*`, maybe add actual metadata (maxvel, authors, creation date)
- zones: custom zone names for bonus credits or maps like classics, progress
