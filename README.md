CS GO observer camera path
===================

Config files for CS GO observer. Generic settings, binds, camera location binds for many maps etc.

Developed for cybermed1a observer.

Originally a fork of baabelfish's observer config, nowadays pretty standalone.

# Installation
1. Go to csgo's cfg directory:  (On windows: *C:\Program Files (x86)\Steam\steamapps\common\Counter-StrikeGlobal Offensive\csgo\cfg*)
2. Clone the contents of the repo under a folder named *caster*:


# Usage
- From console run `exec caster/caster`
- After above, `caster_map_<map>` (*e.g. caster_map_d2*) to load camera binds for individual map
- `caster_map_clear` to clear map specific binds (*or exec caster/pos_clear*)


## Binds

- `F6` - Toggle console (**Note**: default console key is unbound)

### Regular observer binds
- `numbers 1-0` - Switch to player number
- `Left ALT` - Follow nades
- `c` - Auto director
- `x` - Toggle X-ray
- `ctrl` or `q` - big map
- `TAB` - Scoreboard

### Camera control binds

After loading the map config, following binds should work:

##### Static overhead camera angles

- `Keypad 0` - CT base
- `Keypad ,` - T base
- `Keypad 1,4,7` - A site angles / pathways to A
- `Keypad 2,5,8` - Mid angles
- `Keypad 3,6,9` - B site angles / pathways to B

More specific camera locations and other documentation can be found from 
file *guide.txt* or from the map specific config file comments.

##### 5 second lerps to above angles
Switching first to a static camera angle before lerping is recommended.
- `Arrow down` + corresponding key from above

##### Pre defined few second lerps
Do a lerp in a pre defined location on the map (the duration varies from 7 to 14 seconds).
Pressing (and holding) down the key moves the camera to the starting position. Releasing the key starts the actual lerp.
- `v` - CT base
- `b` - T base
- `j` - Mid, or some other part of the map
- `n` - A site
- `m` - B site

### Other binds

#### Shorthands for loading the camera controls for the maps

To avoid using `caster_map_<map>` aliases described above, these binds can be used instead for switching the map on the fly.

- `Insert` - de_inferno
- `Home` - de_mirage
- `PgUp` - de_dust2
- `Delete` - Same as *exec caster/caster*. Clear all the map specific binds and reload the config
- `End` - de_ancient
- `PgDown` - de_overpass
- `]` - de_vertigo
- `[` - de_nuke

#### Sounds

- `Keypad Enter` - Toggle volume on/off

#### HUD binds
Some binds for hiding/showing some HUD elements.

- `Keypad *` - Hide/show player lists from the HUD
- `Keypad -` - "Draw only deathnotices" - Hide/show all of the HUD except the kill feed

Using static camera angles or lerps also tend to hide some HUD elements. 

#### GOTV connect aliases and binds
These aliases and binds are shorthands for joining gotv servers.
The binds can be used to switch a server on the fly but they only work in-game. In the main menu, only aliases can be used.

##### Aliases (type in console)
- `server<number>` - Replace <number> with an integer (currently 1-5), e.g. `server1`
- `akl<number>` - Shorthand of above for AKL

##### Binds
- Hold down `Arrow up` and press an `F-key` (currently `F1`-`F5` are bound)


# Todo
- Add caster_help cfg

