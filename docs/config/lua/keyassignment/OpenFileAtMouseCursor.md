# `OpenFileAtMouseCursor`

If the current mouse cursor position is over a cell that contains
a file path, this action causes that file to be opened in your default editor.

```lua
config.mouse_bindings = {
  -- Ctrl-click will open the file path under the mouse cursor with your default editor
  {
    event = { Up = { streak = 1, button = 'Left' } },
    mods = 'CTRL',
    action = wezterm.action.OpenFileAtMouseCursor,
  },
}
```
