# The Plugin Manifest
In order for The 5zig Mod to recognize and load your plugin, you have to include a JSON file called `plugin.json` inside your jar.

## Plugin Manifest Specification
The manifest should be a dictionary with the following entries:

| Name        | Required?                 | Type     | Description                                                                                                                                               | Example                           |
| ----------- | ------------------------- | -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------- |
| `main`      | Yes                       | `String` | The main class of the plugin.                                                                                                                             | `com.example.ExamplePlugin`       |
| `name`      | Required with `updateUrl` | `String` | The name of the plugin.                                                                                                                                   | `Example Plugin`                  |
| `version`   | Required with `updateUrl` | `String` | The version of the plugin.                                                                                                                                | `1.0.0`                           |
| `author`    | No                        | `String` | The authors of the plugin.                                                                                                                                | `John Doe, Jane Doe`              |
| `desc`      | No                        | `String` | A brief description of the plugin.                                                                                                                        | `An example plugin.`              |
| `license`   | No                        | `String` | The license of the plugin.                                                                                                                                | `MIT`                             |
| `updateUrl` | No                        | `String` | A URL that will be used for automatic updates. Omitting this will disable that feature. See [Automatic Updates](/client-api/updates.md) for more details. | `https://example.com/update.json` |
| `icon`      | No                        | `String` | A URL pointing to a (preferably) 32x32 PNG icon.                                                                                                          | `https://example.com/icon.png`    |

Putting all these values will result in:

```json
{
  "main": "com.example.ExamplePlugin",
  "name": "Example Plugin",
  "version": "1.0.0",
  "author": "John Doe, Jane Doe",
  "desc": "An example plugin.",
  "license": "MIT",
  "updateUrl": "https://example.com/update.json",
  "icon": "https://example.com/icon.png"
}
```