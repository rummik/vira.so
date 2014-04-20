 [Vira](http://vira.so)
========================
Vira will be an augmented reality game revolving around capturing and battling
virtual monsters ('Vira') with friends, other players in your area, and players
across the globe.


## The Algorithm™
Vira are procedurally generated using a stateless algorithm.  This helps with
horizontal scaling, and also lets us safely move a lot of the work off to the
client, and just use the server for verification.

After a Vira is created it shifts location every 3-15 seconds in a 3-5ft area
from its previous location for the duration of its existence (5-30 minutes), or
until it's encountered by a player.

### Data sources

- Map data
  - Used as the environment for exploring and battling with Vira
  - Open StreetMap is probably the best bet for this
- Population data
  - Some types of Vira like being around people more than others, and some
    types don't like being around people
  - From the US it looks like this is freely available from census.gov
- Weather data
  - All the things influence what kinds of Vira appear
  - Forecast.io has a nice (inexpensive) looking API for this

<!--
  We may have invented The Algorithm.  The Algorithm consistently finds Vira.
  The Algorithm creates Vira.  The Algorithm is stateless.  The Algorithm is
  not from Jersey.  The Algorithm consistently finds Vira.  This is not The
  Algorithm. This is close.
-->


## Types of Vira

- Water
- Wind / Air
- Ice
- Fire
- Metal
- Light
- Dark
- Earth / Rock
- Dirt / Ground
- Plant
- Electric
- Poison


<!-- TODO: make note of the glitch and viral attributes somewhere -->
