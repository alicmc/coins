# Blender Command Quick Reference

This guide covers essential Blender shortcuts and tools specifically useful for preparing models for 3D printing.

---

## Navigation

| Keybind      | Action             | Description                     |
| ------------ | ------------------ | ------------------------------- |
| MMB          | Orbit View         | Rotate around object            |
| Shift + MMB  | Pan View           | Move view side to side          |
| Scroll Wheel | Zoom               | Zoom in/out                     |
| Numpad `1`   | Front View         | Front orthographic view         |
| Numpad `3`   | Side View          | Right orthographic view         |
| Numpad `7`   | Top View           | Top orthographic view           |
| Numpad `5`   | Perspective Toggle | Switch perspective/orthographic |
| `.` (Period) | Focus Selected     | Zoom to selected object         |

- to move camera freely using WASD, press Shift+`
  - press Enter to save camera location, Esc to go back to old location
  - press 0 on numpad to reset camera to initial location
  - if the camera is moving too fast for you, change the movement speed in settings (look this up)

---

## Object Mode

| Keybind        | Action    | Description                                 |
| -------------- | --------- | ------------------------------------------- |
| `Shift + A`    | Add Mesh  | Add primitive shapes (cube, cylinder, etc.) |
| `G`            | Move      | Move object                                 |
| `R`            | Rotate    | Rotate object                               |
| `S`            | Scale     | Scale object                                |
| `Shift + D`    | Duplicate | Copy object                                 |
| `Ctrl + J`     | Join      | Combine multiple objects                    |
| `X` / `Delete` | Delete    | Remove object                               |

---

## Edit Mode (Mesh Editing)

> Press `Tab` to enter/exit Edit Mode

| Keybind     | Action      | Description                    |
| ----------- | ----------- | ------------------------------ |
| `1 / 2 / 3` | Select Mode | Vertex / Edge / Face selection |
| `E`         | Extrude     | Extend geometry                |
| `S`         | Scale       | Resize selection               |
| `G`         | Move        | Move selection                 |
| `R`         | Rotate      | Rotate selection               |

---

## Precision & Alignment (IMPORTANT for 3D Printing)

| Keybind         | Action          | Description                     |
| --------------- | --------------- | ------------------------------- |
| `G/R/S + X/Y/Z` | Axis Constraint | Lock transform to axis          |
| `Shift + Tab`   | Toggle Snapping | Enable snapping                 |
| `Shift + S`     | Snap Menu       | Snap to grid, cursor, etc.      |
| `N`             | Transform Panel | Manually input exact dimensions |

---

## 3D Printing Essentials

| Tool / Shortcut                  | Use Case                              |
| -------------------------------- | ------------------------------------- |
| Apply Scale (`Ctrl + A → Scale`) | Ensures correct real-world dimensions |
| `Solidify Modifier`              | Add thickness to thin models          |
| `Boolean Modifier`               | Combine/subtract shapes               |
| `3D Print Toolbox`               | Check for non-manifold edges & errors |

---

## ⚠️ Common Fixes for Printing

- **Recalculate Normals:**  
  `Edit Mode → A → Shift + N`

- **Merge Overlapping Vertices:**  
  `M → By Distance`

- **Check for Non-Manifold Geometry:**  
  `Select → Select All by Trait → Non-Manifold`

---

## 💡 Best Practices

- Always **apply scale** before exporting
- Keep models **watertight (no holes)**
- Avoid **non-manifold geometry**
- Use **real-world units (millimeters recommended)**  
  → Set in _Scene Properties → Units_

---

## Export for Printing

| Format | When to Use   |
| ------ | ------------- |
| STL    | Most common   |
| OBJ    | If multi-part |

**Export Path:**  
`File → Export → STL`

---

## Pro Tips

- Use **orthographic view (Numpad 5)** for accurate alignment
- Model with the **grid as your reference**
- Keep geometry **simple and clean** to avoid slicer errors

---
