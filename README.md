## ElementHotkey
This was forked from [Kushview Element](https://github.com/kushview/element).

## Features
- This software adds shortcut keys to kushview element nodes.
- The concept is based on two options: mouse-only or keyboard shortcuts.

### Basic Functions
- Simultaneously connect or disconnect
- Disconnect the top or all connections
- Toggle on/off (at the selected location)
- Duplicate

## Keyboard Shortcuts
| Action | 🖱️Mouse Shortcut | ⌨️Keyboard Shortcut |
| :--- | :--- | :--- |
| Connect/**Disconnect All** | `Right-click and drag` | `Alt` + `Left-click and drag` |
| Disconnect Top Connections | `Long-press Middle Button` | `Alt` + `Left-click` |
| Disconnect All Connections | `Long-press Middle-Right Click` | `Alt` + `Left-click` |
| Toggle On/Off | `Middle-click` | `Shift` + `Left-click` |
| Duplicate | `None` | `Ctrl` + `Right-click` |

<details>
  <summary><b>🎬 Demo Mouse GIF</b></summary>
  <br>
  <img width="600" alt="ElementHotkey-mouse" src="https://github.com/user-attachments/assets/43215a2f-5a27-4989-85b6-f30d25335921" />
  <p>⚠️Missing GIF⚠️: You can disconnect lines simultaneously by right-dragging a connected line.</p>
</details>
<details>
  <summary><b>🎬 Demo Keyboard GIF</b></summary>
  <br>
  <img width="600" alt="ElementHotkey-mouse" src="https://github.com/user-attachments/assets/f46da1b4-dd9a-4748-ab92-3a43b0498aaa" />
  <p>⚠️Missing GIF⚠️: You can disconnect lines simultaneously by holding down the Alt key while dragging a connected line</p>
</details>

## Caution
Original element version: v1.2.0

- VST / VST2: **Not** supported
- VST3: Supported
- ASIO: Supported
- Architecture: x86-64 only

---



### Modified Source Files
the following files were modified to implement these features:
- `./src/ui/block.cpp` (`:549 mouseDown`, `:723 timerCallback`, `:844 mouseUp`)
- `./src/ui/block.hpp`
- `./src/ui/grapheditorcomponent.cpp` (`:261 mouseDrag`, `:969 endDraggingConnector`)

- The middle button long press is set to 400 ms

## License / Acknowledgements

This software is a custom modification (fork) of [Kushview Element](https://github.com/kushview/element).

- **Original Project:** [Kushview Element](https://github.com/kushview/element) (Copyright (c) Kushview, LLC)
- **License:** Distributed under the [GPL v3 License](LICENSE) (or original license).

This project is not officially affiliated with or endorsed by Kushview, LLC.
