# Config reference for AmmoType (extends [BaseType](BaseType.md))

For each type, the table will list each config and potentially its purpose and default values.

| Keyword             | Type                                | Default                            | Purpose                                                                                             |
|---------------------|-------------------------------------|------------------------------------|-----------------------------------------------------------------------------------------------------|
| numBullets          | int                                 | 1                                  | Number of bullets fired per shot.                                                                   |
| ammoCapacity        | int                                 | 30                                 | Ammo capacity amount.                                                                               |
| magazineCount       | Integer                             | -                                  | Magazine count.                                                                                     |
| reloadTime          | float                               | -                                  | Number of seconds it should take to reload.                                                         |
| recoilPitch         | float                               | 0.0F                               | Base value for upwards cursor/view recoil.                                                          |
| recoilYaw           | float                               | 0.0F                               | Base value for left/right cursor/view recoil.                                                       |
| bulletDamage        | float                               | 1                                  | Damage inflicted per bullet, multiplied by the gun damage value.                                    |
| bulletSpread        | float                               | -                                  | The amount that bullets spread out when fired.                                                      |
| emptyOnCraft        | boolean                             | false                              | Will this ammo item be loaded or empty when crafted?                                                |
| allowEmptyMagazines | boolean                             | true                               | Override ammo deletion, to allow for enabling or disabling of returned empty magazines.             |
| refillCost          | [JsonItemStack](JsonItemStack.md)[] | \[{"id": "gunpowder", "count": 2}] | Cost to refill this magazine, per each missing bullet. Set to `null` to disable magazine refilling. |
| subAmmo             | String[]                            | -                                  | The ammo type(s) that can be loaded into this item.                                                 |
| potionEffects       | [PotionEntry](PotionEntry.md)[]     | -                                  | Array of potion effects applied to an entity upon bullet impact.                                    |
| explosionSize       | Integer                             | null                               | When set and greater than zero, this will cause an explosion on impact with a block.                |