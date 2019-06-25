# Automatic Updates
If you would like to make your plugin update automatically when a new release is available,
you have to include an `updateUrl` in the [plugin manifest](../manifest).

!!! warning
    Users can toggle auto-updating off, so keep in mind this won't always work.

That URL should point to a valid JSON file with the following entries:

| Name | Type | Description | Example |
| ---- | ---- | ----------- | --------|
| `latest` | `String` | The latest version of the plugin | `1.1.0`
| `download` | `String` | The download URL of the latest version | `https://example.com/latest.jar`

For example:

```json
{
    "latest": "1.1.0",
    "download": "https://example.com/latest.jar"
}
```
