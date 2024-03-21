# EXWPack.info

## This file defines basic metadata for your content pack.

Having an exwpack.info file will be required as of v1.2.0 for your content pack to be loaded.

| Keyword           | Type     | Default | Required           | Explanation                                                                                                                                                                                                                           |
|-------------------|----------|---------|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| packId            | String   | -       | :heavy_check_mark: | This pack's **unique** identifier.<br/>In the future, content packs will not be loaded without this field. Please make sure it is a unique ID value. Must be all lowercase, with no spaces.                                           |
| authorList        | String[] | []      |                    | List of authors for this pack.                                                                                                                                                                                                        |
| url               | String   | ""      |                    | URL for this pack's website.                                                                                                                                                                                                          |
| version           | String   | 1.0.0   |                    | Pack version.                                                                                                                                                                                                                         |
| logo              | String   | ""      |                    | Logo file.                                                                                                                                                                                                                            |
| name              | String   | ""      |                    | Name of this pack.                                                                                                                                                                                                                    |
| credits           | String   | ""      |                    | Credits for this pack.                                                                                                                                                                                                                |
| ~~buildRevision~~ | Integer  | -       |                    | The target API revision.<br/><br/>**Deprecated:** Please update to _targetAPI_.                                                                                                                                                       |
| targetAPI         | String   | -       | :heavy_check_mark: | The target API version this pack is made for. Please consult the [dev page](https://exw.rainyville.org/dev/api-targets) for more details. Leaving this field blank while specifying `buildRevision` will default to Target API 1.0.0. |
| dependencies      | String[] | []      |                    | List of content pack dependencies. List content packs by their pack ID, EXW will verify they are present during load time.                                                                                                            |

This file should be in the root directory of your content pack.
If it cannot be located at runtime, default values will be used.

It will still be loaded from Flan's or Modulus compatible content packs.