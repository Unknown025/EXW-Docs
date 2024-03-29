# Config reference for BaseType

For each type, the table will list each config and potentially its purpose and default values.

| Keyword           | Type                      | Default           | Purpose                                                                                                                                                              |
|-------------------|---------------------------|-------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| modelName         | String                    | -                 | Name of the model for this item.                                                                                                                                     |
| ~~modelLocation~~ | String                    | -                 | Location of the Wavefront OBJ file, stemming from "assets/exw/wavefront/\<object type>/"<br/>**Deprecated:** Use `modelName` to specify the name of your model file. |
| ~~loadWavefront~~ | Boolean                   | false             | Whether this type should try to load a Wavefront OBJ model from `modelLocation`.<br/>**Deprecated:** Use `ModelType` to determine which type of model this item has. |
| modelType         | [ModelType](ModelType.md) | ModelType.TOOLBOX | Determines which type of model will be loaded.                                                                                                                       |
| maxStackSize      | Integer                   | -                 | The maximum stack size for this item. (If not specified, a default value will be used depending on the type.)                                                        |
| modelSkins        | [SkinType](SkinType.md)[] | -                 | The skins available for this item.                                                                                                                                   |
| internalName      | String                    | -                 | The unlocalized name for this item.                                                                                                                                  |
| displayName       | String                    | -                 | The display name for this item.                                                                                                                                      |
| iconName          | String                    | -                 | The name of the icon for this item.                                                                                                                                  |