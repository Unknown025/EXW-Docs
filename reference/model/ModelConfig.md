# Config reference for Wavefront OBJ models

For each type, the table will list each config and potentially its purpose and default values.

| Keyword               | Type                                     | Default | Required | Explanation |
|-----------------------|------------------------------------------|---------|----------|-------------|
| customOrigins         | HashMap<String, [Vector3f](Vector3f.md)> | -       |          | -           |
| renderTransformations | [ModelTransform](ModelTransform.md)[]    | -       |          | -           |
| modelScale            | float                                    | 1F      |          | -           |

# Example config
```json
{
  "modelScale": 0.9,
  "customOrigins": {
    "FrontLeftWheel": {
      "x": 0.92842,
      "y": -0.57389,
      "z": 1.7016
    },
    "FrontRightWheel": {
      "x": -0.92842,
      "y": -0.57389,
      "z": 1.7016
    },
    "RearLeftWheel": {
      "x": 0.92842,
      "y": -0.57389,
      "z": -1.4386
    },
    "RearRightWheel": {
      "x": -0.92842,
      "y": -0.57389,
      "z": -1.4386
    }
  },
  "renderTransformations": [
    {
      "type": "TRANSLATE",
      "vector": {
        "x": 0,
        "y": 0.95,
        "z": -0.1
      }
    },
    {
      "type": "ROTATE",
      "angle": 90,
      "vector": {
        "x": 0,
        "y": 1,
        "z": 0
      }
    }
  ]
}
```