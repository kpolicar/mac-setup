# macOS Windows-ify Setup Prompts

Give these prompts to an LLM on your new Mac to recreate your current environment.

### 1. The Core Setup (Apps & Keys)
"Install Homebrew, then use it to install: **karabiner-elements**, **alt-tab**, **rectangle**, and **linearmouse**. 

In Karabiner-Elements:
- Import and enable the **'Windows shortcuts on macOS'** complex modification from: `https://ke-complex-modifications.pqrs.org/?q=Windows%20shortcuts%20on%20macOS#windows_shortcuts_on_macos`
- Add a custom rule to map **Ctrl + F4** and **Cmd + F4** (including the **Search/Spotlight** key) to **Cmd + W**.
- In 'Simple Modifications', remap the **Fn (Globe)** key to **Left Command**."

### 2. Chrome & System Cleanup
"Ensure no system-level App Shortcuts (NSUserKeyEquivalents) are mapping F4 to 'Close Tab' in Chrome to avoid beeping conflicts. Check the 'System Settings > Keyboard > Keyboard Shortcuts > Mission Control' section and ensure 'Move focus to the next window' is disabled, as it blocks Ctrl + F4."

### 3. Mouse & Window Snapping & Alt-Tab
"Configure **LinearMouse** to invert the mouse wheel scroll direction while keeping the trackpad scrolling 'Natural'. Configure **Rectangle** with standard Windows-style shortcuts for half-screen and full-screen snapping. 

For **Alt-Tab**, configure it to show windows from **all spaces and screens**, and ensure the trigger shortcut uses the **Command** key (matching the remapped Fn key) to feel like Windows Alt+Tab."

---

## Manual System Settings (Mandatory)
*These must be toggled by hand for the shortcuts to work:*

1.  **Permissions:** Grant **Input Monitoring**, **Accessibility**, and **Screen Recording** (for Alt-Tab) permissions to the new apps in System Settings.
2.  **Mission Control Conflict:** Go to *Settings > Keyboard > Keyboard Shortcuts > Mission Control* and **uncheck** "Move left/right a space" and "Move focus to the next window" (this is why Ctrl+F4 and Ctrl+Arrows often fail).
3.  **Fn Key Behavior:** Go to *Settings > Keyboard* and set "Press Fn key to" to **Do Nothing** (so Karabiner can use it as Command).
