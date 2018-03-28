Field documentation for the Ur-Quan Masters planet database
CSV dump format.

By Scott A. Colcord (Elestan on http://forum.uqm.stack.nl)

29 Jun, 2011

Cluster:
  Name of the star's cluster.

Star:
  Name of the star.  "Prime" if there is only one in the cluster.

X,Y:
  Coordinates of the star.

DistSol:
  Distance from Sol.

StarColor:
  Color of the star.

StarSize:
  dwarf, giant, or super giant.

Fleet:
  The closest fleet whose sphere of influence includes the system, if any.

Planet:
  Name of the planet.  Just a Roman numeral for unnamed planets.  
  Moons add a suffix.

Type:
  Type of the planet (e.g. "Gas Giant")

Hazard:
  This value is an aggregate estimate of how dangerous the planet is to land
  on.  It is computed from the tectonics, weather, temperature, and bioHazard
  ratings, and tries to combine them in a way that follows the calculations
  in the code.  For example, when one looks at the hazard event probabilities,
  two level 3 hazards are roughly equivalent to a level 4 hazard, and three 
  level 4 hazards are roughly equivalent to a level 5 hazard.

Tectonics:
  The tectonic hazard level, as displayed to the user.

Weather:
  The weather hazard level, as displayed to the user.

Thermal:
  The thermal hazard level.  This value is derived from Tempoerature, and is
  used in the code in the same manner as Tectonics and Weather, even though 
  it's never shown to the user.

BioHazard:
  This is the approximate threat level of the nastiest lifeform on the planet.
  It is scaled to a 1-8 range to match the other hazards.

BioUnits:
  The total units of BioData available on the planet.  Note that this is not
  the Credit value of the BioData (which is what the human-readable dump
  provides).

MinValue:
  The total value of all minerals on the planet.

MinVolume:
  The total number of mineral units on the planet.  Each cargo hold in the
  flagship holds 500 units.

Fuel:
  The fuel required for one lander round trip to the planet.

AxialTilt,Density,Radius,Gravity,Temp,Day,Atmosphere,LifeChance,DistFromStar:
  All of these values come from the planet database, and do not directly
  affect gameplay other than by figuring into other values that do.
  For example, Gravity determines fuel, Atmosphere determines weather,
  DistFromStar determines temperature, which determines thermal hazard, etc.

