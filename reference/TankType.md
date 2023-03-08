# Config reference for TankType (extends [VehicleType](VehicleType.md))

For each type, the table will list each config and potentially its purpose and default values.

| Keyword           | Type                       | Default        | Purpose                                                                                                    |
|-------------------|----------------------------|----------------|------------------------------------------------------------------------------------------------------------|
| barrelOrigin      | [Vec3f](model/Vector3f.md) | -              | Sets the origin of the tank's barrel (used for calculating where the raytracing should be projected from). |
| explosionStrength | float                      | 12F            | Strength of an explosion caused by impacting a block.                                                      |
| fireDelay         | int                        | 60 (3 seconds) | Amount of ticks between a player being able to fire again.                                                 |
| maxBarrelAngle    | float                      | 25F            | Maximum angle the barrel can pivot.                                                                        |
| minBarrelAngle    | float                      | -5F            | Minimum angle the barrel can pivot.                                                                        |
| damage            | float                      | 12F            | Amount of damage this tank deals.                                                                          |
| damageTerrain     | boolean                    | true           | Whether terrain is damaged upon hitting a block.                                                           |