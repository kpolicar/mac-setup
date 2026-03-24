# macOS Windows-ify Setup Prompts

Give these prompts to an LLM on your new Mac to recreate your current environment.

### 1. The Core Setup (Apps & Keys)
"Install Homebrew, then use it to install: **karabiner-elements**, **alt-tab**, **rectangle**, and **linearmouse**. 

In Karabiner-Elements, create a profile with these rules:
- **Simple Modifications:** Remap **Fn (Globe)** key to **Left Command**.
- **Word Navigation:** Map both **Cmd + Arrows** and **Ctrl + Arrows** to **Option + Arrows** (moves cursor by word).
- **Snapping Trigger:** Map **Option + Arrows** to a hidden combination like **Cmd + Ctrl + Shift + Arrows**. This 'frees up' Option+Arrows for window snapping without moving the cursor or changing brightness.
- **Close Tab:** Map **Ctrl + F4** and **Cmd + F4** (including Search/Spotlight/Launchpad keys) to **Cmd + W**.
- **Delete Word:** Map **Ctrl + Backspace** and **Cmd + Backspace** to **Option + Backspace**."

### 2. Window Snapping & Alt-Tab
"Configure **Rectangle** to use **Option + Arrows** for snapping (Left, Right, Maximize/Up, Bottom/Down). Because of the Karabiner mapping, these will snap windows without moving the cursor.

For **Alt-Tab**, configure it to show windows from **all spaces and screens**, and set the trigger shortcut to the **Command** key (which will be your remapped Fn key)."

### 3. Mouse & System Cleanup
"Configure **LinearMouse** to invert the mouse wheel scroll direction while keeping the trackpad 'Natural'. 

In macOS System Settings:
- Go to *Keyboard > Keyboard Shortcuts > Mission Control* and **uncheck** 'Move focus to the next window' (this blocks Ctrl+F4).
- Also **uncheck** 'Move left/right a space' (this blocks Ctrl+Arrows).
- Set 'Press Fn key to' to **Do Nothing** in Keyboard settings."

---

## Manual Permissions (Mandatory)
Grant **Input Monitoring**, **Accessibility**, and **Screen Recording** (for Alt-Tab) permissions to the new apps in System Settings as prompted.
