# Weather Radar Database

 The database of world weather radars. Structure of `weather-radar-database.json` file:

* `id` - radar identifier
* `codes` - other radar codes (identifiers)
    * `wmo` - World Meteorological Organization code
    * `ccid` - Old country ID code
    * `ccccii` - New country ID code
    * `icao` - International Civil Aviation Organization airport code
* `location` - city or place when weather radar is located
* `state` - abbreviation or name of radar's location state
* `country`- country in which this weather radar located
* `status` - 1 - operated, 0 - not operated
* `latitude` - latitude of weather radar coordinates (WGS 84)
* `longitude` - longitude of weather radar coordinates (WGS 84)
* `max_range` - maximum weather radar range
* `antenna` - Information about antenna parameters
    * `band` - Wavelength: S ~ 10 cm, C ~ 5 cm, X ~3 cm
    * `polarization` - S - single, D - dual
    * `height` - Height centre of antenna above sea level (meters)
    * `diameter`- Antenna diameter (meters),
    * `beam` - Antenna scan degree (º)
    * `gain` - Antenna gain (dB)
    * `frequency` - Operation frequency (GHz)
* `station` - Details about weather radar site
    * `start_year`- Year of weather radar site deployment
    * `height` - Height of basis of tower
    * `wrwp` - Can produce weather radar wind profile: `1` - yes, `0`- no