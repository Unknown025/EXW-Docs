# Config reference for VehicleType (extends [BaseType](BaseType.md))

For each type, the table will list each config and potentially its purpose and default values.

| Keyword                    | Type                                                                         | Default      | Purpose                                                            |
|----------------------------|------------------------------------------------------------------------------|--------------|--------------------------------------------------------------------|
| rotateWheels               | boolean                                                                      | false        | Whether the front wheels should be rotated.                        |
| ~~turretOrigin~~           | Vector3f                                                                     | -            | Origin of the vehicle's turret (if applicable).<br/>**Deprecated** |
| ~~primaryWeaponVectors~~   | Vector3f[]                                                                   | -            | -<br/>**Deprecated**                                               |
| ~~secondaryWeaponVectors~~ | Vector3f[]                                                                   | -            | -<br/>**Deprecated**                                               |
| seats                      | [SeatInfo](SeatInfo.md)[]                                                    | -            | Seats for this vehicle.                                            |
| width                      | float                                                                        | 2            | Width of the vehicle's hitbox.                                     |
| height                     | float                                                                        | 2            | Height of the vehicle's hitbox.                                    |
| ~~leftTrackVectors~~       | Vector3f                                                                     | Vector3f\[0] | Left track vectors.<br/>**Deprecated**                             |
| ~~rightTrackVectors~~      | Vector3f                                                                     | Vector3f\[0] | Right track vectors.<br/>**Deprecated**                            |
| ~~trackLinkLength~~        | float                                                                        | 0            | Track link length.<br/>**Deprecated**                              |
| ~~trackLinkFix~~           | int                                                                          | 5            | -<br/>**Deprecated**                                               |
| ~~flipLinkFix~~            | boolean                                                                      | false        | -<br/>**Deprecated**                                               |
| ~~animationFrames~~        | int                                                                          | 2            | Animation frames.<br/>**Deprecated**                               |
| maxVelocity                | double                                                                       | 0            | Maximum velocity this vehicle can reach.                           |
| allowDefaultSounds         | boolean                                                                      | true         | Whether default ExW sounds are allowed.                            |
| emptyPitch                 | float                                                                        | 0.05F        | -                                                                  |
| vehicleSoundMap            | HashMap<[SoundType](SoundType.md), ArrayList\<[SoundEntry](SoundEntry.md )>> | -            | Vehicle sound map.                                                 |