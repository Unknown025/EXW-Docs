# Config reference for TankType (extends [VehicleType](VehicleType.md))

For each type, the table will list each config and potentially its purpose and default values.

| Keyword           | Type                       | Default        | Purpose                                                                                                   |
|-------------------|----------------------------|----------------|-----------------------------------------------------------------------------------------------------------|
| turretOrigin      | [Vec3f](model/Vector3f.md) | -              | Sets the origin of the tank's turret (used for calculating where the raytracing should be projected from. |
| explosionStrength | float                      | 0              | Strength of an explosion caused by impacting a block.                                                     |
| fireDelay         | int                        | 60 (3 seconds) | Amount of ticks between a player being able to fire again.                                                |