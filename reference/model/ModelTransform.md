# Config reference for ModelTransform

For each type, the table will list each config and potentially its purpose and default values.

| Keyword | Type                    | Default | Required           | Explanation                              |
|---------|-------------------------|---------|--------------------|------------------------------------------|
| type    | TransformType           | -       | :heavy_check_mark: | Defines the type of this transformation. |
| angle   | float                   | 0F      |                    | Used in rotations.                       |
| vector  | [Vector3f](Vector3f.md) | -       | :heavy_check_mark: | Vector to use for this transformation    | 