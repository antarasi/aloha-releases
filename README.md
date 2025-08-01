# aloha-releases
Aloha Desktop Metadata and Release Registry

# How to make your plugin discoverable in Aloha Desktop Agent?

Open `plugins.json` file and create a Pull Request adding an entry with details of your plugin:

```json
[
    ...
    {
        "repo": "username/aloha-repo-name",
        "name": "Display Name",
        "author": "your name",
        "description": "Short description what your plugin does",
        "icon": "https://raw.githubusercontent.com/username/aloha-repo-name/refs/heads/main/public/icon.svg"
    }
]
```

Once your Pull Request is reviewed and merged your plugin will show up on the list of plugins in the app.

> **Note:** You only need to submit the plugin once. After your plugin has been published, users can download and update to new releases from the app.

# Publishing Requirements

1. Published as a release on GitHub - preferably use the [offcial vite based workflow](https://github.com/antarasi/vite-aloha)
1. The repo name must be prefixed with `aloha-`
1. The plugin must be open source
1. No telemetry - respect users privacy