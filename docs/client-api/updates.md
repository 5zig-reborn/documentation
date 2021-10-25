# Automatic Updates
If you would like to make your plugin update automatically when a new release is available,
you have to include an `updateUrl` in the [plugin manifest](/client-api/manifest.md).

!!! info "Note"
    Users can toggle auto-updating off, so keep in mind this won't always work.

## How it works
The URL you set in the `plugin.json` should point to a JSON file which contains the following information:

| Name       | Type     | Description                             | Example                          |
| ---------- | -------- | --------------------------------------- | -------------------------------- |
| `latest`   | `String` | The latest version of the plugin.       | `1.1.0`                          |
| `download` | `String` | The download URL of the latest version. | `https://example.com/latest.jar` |

For example:

```json
{
  "latest": "1.1.0",
  "download": "https://example.com/latest.jar"
}
```
