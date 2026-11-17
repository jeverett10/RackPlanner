# Changelog

All notable changes to the Rack Planner are documented in this file.

## [0.2.1] - 2026-11-17

### Added

- Device settings window for every device, opened from a sliders button in the library, from the selection bar above the rack, by double-click or Enter on a device, from the top-down view, and from the wiring connector panel.
- Editable name, maker, category, height, mounting type, and shelf depth in the settings window.
- Exact width and depth to any decimal, with an inches or millimetres switch that is remembered.
- Per-connector side, type, label, and count, plus optional hand-set position (offset from the left edge for front and rear, from the front edge for the sides) and spacing between connectors in a group.
- New connector types: XLR, 1/4 in TRS/TS, XLR/TRS combo, 3.5 mm jack, RCA, MIDI (5-pin DIN), SDI, speakON, powerCON, and DB25.
- Warning in the settings window when removing a connector would delete cables attached to it.
- "Add your own gear" now opens the full settings window, and saved library items keep their maker, category, and connectors.
- Click-to-select for rack devices and shelf items, with a selection bar offering Move up, Move down, Taller, Shorter, Top-down view, Device settings, Remove, and Deselect.
- Multi-select in the rack with Shift- or Ctrl/Cmd-click, a Select all button, and Ctrl/Cmd+A.
- Group move up and down in the rack by button, arrow keys, or drag. A blocked group hops over the obstruction to the next free spot.
- Drag-and-drop of a multi-selection in the rack, with ghosts, green and red drop outlines, cross-bay moves, drop-on-library to remove, and Esc to cancel.
- Multi-select on a shelf in the top-down view with Shift- or Ctrl/Cmd-click and a Select all button.
- Group drag, arrow-key nudge, rotation (about the group's centre, with the group slid back inside the shelf if it swings past an edge), and removal in the top-down view.
- Taller and Shorter buttons to resize shelves, drawers, blank panels, and other rack items by one rack unit without rebuilding the shelf. Growth falls back to downward when there is no room above.
- Pull-out shelf, 1U and 2U, in the Shelves library group.

### Changed

- Shrinking the rack now slides gear down by exactly the amount it overhangs, bay by bay. Growing the rack leaves gear where it is. The change is refused only if the gear cannot fit even after sliding down.
- Connector positions now feed the top-down view and the cable length estimates, so hand-set positions are respected in both.
- Connector count limit raised from 24 to 48 per entry.
- The generic connector type is now labelled "Other connector".
- Escape no longer closes the top-down view while a dialog is open.
- Clicking a library button no longer switches the rack to the rear view for rear-mounted gear.

### Fixed

- Renaming a rack device, or changing its maker, height, or category, now updates its front panel immediately.

## [0.1.0] - 2026-11-12

### Added

- Drag-and-drop rack elevation with a searchable, collapsible gear library, U-height tracking, and custom gear entry.
- Waves SoundGrid servers (Extreme Server-C, Server One-C, Impact Server, SuperRack LiveBox), with half-rack mounting and shared-row logic.
- Waves Live Box and Axis Scope, Sonnet RackMac mini, and DiGiGrid MGO.
- Rack shelves that hold loose or half-rack gear, with a top-down shelf layout view and drag positioning.
- Free 360-degree rotation of shelf items with a drag handle.
- Connector modeling (face, type, label, count) with visual markers on devices.
- Wiring view with device cards, connector pins, drag-to-connect cables, auto-arrange, and a cable list.
- Cable length estimates with a global service-loop setting, per-cable slack adjustment, manual override, and an order summary grouped by type and length.
- PDF export covering the rack elevation, shelf plans, wiring diagram, and cable schedule.
- Marquee selection, mass delete, and undo for cables, plus shift-click selection and group drag for wiring cards.
- Double-wide and triple-wide racks (multiple bays), standard, angled studio (slant), and shock-mount rack styles, casters, an optional top shelf, and an optional storage base.
- Angled rack face with adjustable angle (10 to 45 degrees), plus a matching side view in the app and in the PDF.
- 32 more library items (Shure wireless, dbx, Yamaha, Furman, APC, amplifiers, patch bay), then DiGiCo SD-Rack family, SSL Network I/O, grandMA3 lighting processors and nodes, more rack-mount Mac and Windows computers, patch panels, blank, vent, and brush plates, rear-mounted lacing bars with a front and rear view toggle, and drawers.
- Save/Open project files (JSON) and a standalone-browser download fallback, so the tool works outside the chat.

### Changed

- Auto-arrange in the wiring view is connection-aware, with hubs and spokes, automatic card mirroring, column splitting for rear-to-rear cable chains, and cable-count-aware spacing.
- Cables are routed orthogonally on separate lanes with rounded corners, and clicking or dragging dims everything but the focused cables.
- The slant rack was rebuilt as a fully angled rack face instead of an angled top section, to match real products such as the Gator Elite Series Angled 12U Studio Rack and the RAB Audio ProRak 16U.

### Fixed

- Wiring cards that had become impossible to drag.



The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

