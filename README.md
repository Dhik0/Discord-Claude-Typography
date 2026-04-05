# Discord-Claude-Typography
A lightweight solution to replace Discord fonts with Claude style using betterdiscord.



⚠️ Important: Before You Start
To ensure the CSS applies correctly and to allow for troubleshooting, please check your BetterDiscord Settings:

Enable DevTools: Go to Settings > BetterDiscord > Settings and toggle DevTools to ON. This allows you to use Ctrl+Shift+I (or F12) to inspect elements and force-inject styles if the GUI hangs.

Enable Inspector Shortcut: (Optional but recommended) Toggle Inspector Shortcut to ON. This helps you quickly identify the exact CSS classes if Discord updates their UI again.

Restart Discord: After changing these settings, press Ctrl + R to refresh the client and ensure the injection engine is active.

# Discord Claude.ai Typography Patch (2026)

Restore your reading experience. This is a lightweight, "zero-maintenance" CSS snippet that brings the premium, book-like typography of Claude.ai directly into your Discord chat.

### Why This Project?
Most Discord themes break whenever the official app updates. This patch uses "Magic Selectors"to bypass Discord's 2026 class-name obfuscation (hashing), ensuring your styles stay intact while others fail.

### Key Features
- Specifically tuned `line-height` (1.75) and `letter-spacing` for deep reading.
- Uses `[class^="markup_"]` to precisely hit message content without ruining the UI.
- Looks stunning on high-resolution displays (like ROG Strix / 2K+ screens).
- Just a few lines of CSS. No bulky theme files required.

### Quick Start
1. Open BetterDiscord  or Vencord settings.
2. Go to Custom CSS.
3. Paste the code from `discord-claude.css` in this repo.
4. Hit Save and enjoy.

###  Technical Logic (For Devs)
The snippet leverages attribute wildcard selectors to target dynamically generated Webpack classes:
- `[class^="markup_"]`: Matches any class starting with `markup_`.
- `[class*="messageContent-"]`: Ensures fallback for different Discord versions.

###  Get the Code
You can find the CSS file here: [claude-typography.css](./claude-typography.css)
---
*Created by a developer who just wanted to read Discord messages like a pro.*
