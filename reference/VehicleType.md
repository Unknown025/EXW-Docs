# Config reference for VehicleType (extends [BaseType](BaseType.md))

For each type, the table will list each config and potentially its purpose and default values.

| Keyword            | Type                                                                         | Default | Purpose                                                                                                              |
|--------------------|------------------------------------------------------------------------------|---------|----------------------------------------------------------------------------------------------------------------------|
| rotateWheels       | boolean                                                                      | false   | Whether the front wheels should be rotated.                                                                          |
| seats              | [SeatInfo](SeatInfo.md)[]                                                    | -       | Seats for this vehicle.                                                                                              |
| width              | float                                                                        | 2       | Width of the vehicle's hitbox.                                                                                       |
| height             | float                                                                        | 2       | Height of the vehicle's hitbox.                                                                                      |
| maxVelocity        | double                                                                       | 15D     | Maximum velocity this vehicle can reach.<br/>**Deprecated:** Maximum velocity is now determined by #gearDefinitions. |
| maxReverse         | double                                                                       | 5D      | Maximum reverse speed for this vehicle.                                                                              |
| acceleration       | double                                                                       | 1D      | Acceleration modifier, applied for each tick a vehicle is accelerating.                                              |
| allowDefaultSounds | boolean                                                                      | true    | Whether default vehicle sounds are allowed.                                                                          |
| emptyPitch         | float                                                                        | 0.05F   | -                                                                                                                    |
| gearDefinitions    | double[]                                                                     | -       | Array of maximum speeds for each gear. The more maximum speeds are defined, the more gears a vehicle has.            |
| vehicleSoundMap    | HashMap<[SoundType](SoundType.md), ArrayList\<[SoundEntry](SoundEntry.md )>> | -       | Vehicle sound definitions.                                                                                           |

# Example config
```json
{
  "modelType": "WAVEFRONT",
  "maxStackSize": 1,
  "internalName": "dvg.uaz_469",
  "displayName": "UAZ 469",
  "maxReverse": 10,
  "rotateWheels": true,
  "gearDefinitions": [
    10,
    18.5,
    26,
    35
  ],
  "acceleration": 1.25,
  "seats": [
    {
      "driver": true,
      "xOffset": -0.15,
      "yOffset": 0.2,
      "zOffset": -0.2
    },
    {
      "xOffset": -0.15,
      "yOffset": 0.3,
      "zOffset": 0.2
    },
    {
      "xOffset": -0.75,
      "yOffset": 0.5
    }
  ],
  "modelSkins": [
    {
      "internalName": "dvg.uaz_469",
      "skinAsset": "dvg.uaz_469",
      "displayName": "UAZ 469 - Default"
    },
    {
      "internalName": "dvg.uaz_469.blue",
      "skinAsset": "dvg.uaz_469.blue",
      "displayName": "UAZ 469 - Blue"
    }
  ]
}
```