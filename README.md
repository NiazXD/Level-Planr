# Level Planr

A browser-based planning tool for level designers. Block out a level in **isometric** view (cubes on a multi-level grid) or **top-down** view (floor plans: rooms, furniture, doors), annotate it, and share it as a file or an image. It is one static page with no build step and no dependencies, and it can be installed as an app and used offline.

## Running it

- **Locally:** open `index.html` in a browser.
- **Hosted (GitHub Pages):** repo **Settings → Pages → Deploy from branch → `main` / root**. The site appears at `https://<username>.github.io/Level-Planr/`.
- **As an app:** in a supported browser, use *Install* / *Add to Home Screen*. It works offline after the first visit.

## Getting started

1. Click **New** and choose **Isometric** or **Top-down**. (Top-down starts at 24×16×3 cells, isometric at 12×12×6. Change it any time under *Level & scene → Size*.)
2. Pick a tool from the left toolbox (or press `1`–`9`) and click or drag on the grid.
3. Use the right panel to set colour, snap, gizmo mode and level.
4. **Save** keeps the project in your browser; **Export** downloads a file you can send to someone else.

The **View** button (or `V`) switches the camera between isometric and top-down on any project. The data is the same, only the camera changes.

## Tools

| Key | Tool | What it does |
|---|---|---|
| `1` | Select | Select, move and scale items. Drag empty space to pan. |
| `2` | Cube | Click to place a cube, or **drag on the grid** to draw a wall or room block. Click a cube face to add a cube against it. Height comes from *Cube height*. |
| `3` | Custom | Click to place the vertices of a polygon. Close it by clicking the first point, double-clicking, or pressing `Enter` (`Esc` cancels, `Backspace` removes the last point). |
| `4` | Arrow | Drag to draw an arrow on the current level. |
| `5` | Text | Click to place the text typed in *Labels & icons*. |
| `6` | Dot | Click to place a dot marker. |
| `7` | Icon | Place an uploaded image icon (use *Icons ▾* to upload or choose one). |
| `8` | Door | Click near a grid edge to place a door. |
| `9` | Erase | Click an item to remove it. |
| | Shapes ▾ | Pick a shape (square, circle, triangle, diamond, star, …), then drag on a cube face to draw it. In top-down view you can also draw directly on the floor. |

## Editing

- **Gizmo:** with an item selected, `G` shows the move gizmo, `S` the scale gizmo, `Q` hides it. Cubes, shapes, custom shapes, text and icons can be moved and scaled. Arrows and custom shapes also have draggable handles.
- **Arrows:** drag the end handles of a selected arrow, or use the scale gizmo to change its length.
- **Custom shapes:** with one selected, drag a vertex to move it, click anywhere on an edge to add a vertex, and Shift+click a vertex to remove it.
- **Doors:** a door is a coloured, thin rectangle that sits on a grid edge. It only snaps to grid edges. Drag it to slide it along edges, and change its width in the inspector or the right-click menu.
- **Face mode (`Tab`):** select a single grid square on a cube, then push or pull it to extrude or carve the cube.
- **Right-click** any item for its settings: label, icon, plane, size, width, height, colour, duplicate and delete.
- **Rename:** double-click text or a label, or press `F2`.
- **Labels:** dots, icons and custom shapes can carry a label (for example "Bed" on a custom shape).
- **Levels:** `[` and `]` change the active level. *Slice* fades items that are not on the current level.
- **Snap:** choose 1, ½ or ¼ cell snapping for arrows, doors, custom shapes and labels.

## Sharing and saving

- **Save / Open:** projects are stored in your browser's local storage. They are not uploaded anywhere, and clearing site data removes them.
- **Export / Import:** downloads or opens a `.levelplanr.json` file containing the whole project, including uploaded icons. Send the file to share a project. (Older `.isoplan.json` files also import.)
- **PNG:** exports what you currently see on the canvas as an image.

## Keyboard shortcuts

| Shortcut | Action |
|---|---|
| `1`–`9` | Choose tool (see table above) |
| `G` / `S` / `Q` | Move gizmo / scale gizmo / gizmo off |
| `Tab` | Toggle Object / Face selection |
| `X`, `Delete` | Delete selected |
| `Shift+D` | Duplicate selected |
| `F2` | Rename text or label |
| `Ctrl+Z`, `Ctrl+Shift+Z` / `Ctrl+Y` | Undo, redo |
| `Ctrl+S` | Save project |
| `[` `]` | Level down / up |
| `V` | Toggle isometric / top-down |
| `Numpad 7` / `Numpad 0` | Top-down / isometric view |
| `Home` | Fit scene to window |
| `L` | Toggle slice |
| `Shift+G` | Toggle grid |
| Arrow keys | Nudge the selected item; `PgUp` / `PgDn` move a cube up/down |
| `Esc` | Cancel a custom shape, close a menu, or return to Select |
| `?` | Show this list in the app |

Mouse: wheel to zoom, middle- or right-button drag (or drag empty space with the Select tool) to pan.

## Limitations

- Cubes sit on whole grid cells, so there are no thin walls. Use cubes for walls and doors for openings.
- Everything is stored per browser. Use Export to move projects between devices or people.

## License

No license has been set yet. Add one before inviting contributions.
