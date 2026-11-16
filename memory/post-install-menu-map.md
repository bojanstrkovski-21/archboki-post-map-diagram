# Post-install menu map

`post-install-system-map.md` is the starting point for more work on this system. It maps `03.arch-boki-post-install-gum.sh` and only the scripts that menu opens, down to the last choice.

Read that file before redrawing or extending the map. The script list at the bottom names every file `03` calls. There are 18. `install-scripts/130-archboki-install-apps.sh` does not call any further script. Audio and fonts are the other nested prompts.

Diagram rules:

- Separate Mermaid charts, not one chart.
- `flowchart TD` (top to bottom).
- A rounded node is a menu. A square node is a script, a command, or the last screen before a package table.
- Leave Back, Main Menu, and Quit off every chart.
- Package rows stay in the tables under each chart.
- The font chart stops at Font Installation Manager and its three choices. The numbered font lists stay tables.

The ten charts are Main Menu (four working choices), Update and Refresh, Choose Desktop, Core Utils, Install Apps (eight categories), then Text/office, Internet, Multimedia, Graphics, and System Tools. On the Core Utils chart, audio splits into PipeWire and PulseAudio.

## Files

- `../post-install-system-map.md`
