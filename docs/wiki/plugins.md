# Plugins

A plugin is a separate addon that adds its own module to EldoUI. It gets a settings page in the EldoUI config window, a row on the Plugins page (title, version, author, on/off switch), optional setup pages in the installer, a line in `/eui diag` and the version check. Everything goes through the global `EldoUI`, the same calls EldoUI's own modules use, so a plugin looks and behaves like the rest of the UI.

The smallest plugin is a `.toc` that depends on EldoUI:

```
## Interface: 16001
## Title: My Bars
## Dependencies: EldoUI
```

and a module:

```lua
local M = EldoUI:NewModule("MyBars", {
	title = "My Bars",
	desc = "Two extra bars.",
	plugin = "MyBars",
	defaults = { enabled = true },
})

function M:OnEnable()
	self:Print("Hello from a plugin.")
end
```

Plugins follow the same rules as EldoUI: change how things look and where they sit, show only what the game gives addons, never automate gameplay, and use EldoUI's design kit instead of their own colors and fonts.

## Full guide

The plugin API, the plugin record, settings and setup pages, hooks, the version check and a checklist before you publish are in the [plugin guide](../PLUGINS.md).

In game, `/eui plugins` opens the Plugins page and `/eui plugins list` prints the loaded plugins.
