# Config reference for ModelType

The following are available values that apply to any field requiring parameter `ModelType`.

| Name        | Directory   | File Extension |
|-------------|-------------|----------------|
| TOOLBOX     | -           | -              |
| WAVEFRONT   | `wavefront` | obj            |
| METASEQUOIA | `metaseq`   | mqo            |

## Where your models should go
### Toolbox
Toolbox models go into the Java package `org.rainyville.modulus.client.model`. You can create
your own package, such as `org.rainyville.modulus.client.model.cf`.

### Wavefront
OBJ models go into your content pack's assets folder. For example, if your
content pack is named "Modern Warfare" and you're adding a vehicle model, it would go in
`Modern Warfare/assets/exw/wavefront/vehicles/`.

### Metasequoia
Metasequoia models follow the same format as OBJ models, except instead of "wavefront",
models go into a "metaseq" folder, such as `Modern Warfare/assets/exw/metaseq/vehicles`.