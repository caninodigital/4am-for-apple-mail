<p align="center"><img src="assets/icon.png" width="128" height="128" alt="4AM app icon"></p>

# 4AM for Apple Mail

**Gmail-style keyboard shortcuts for Apple Mail on the Mac.** Press `E` to archive, `J` and `K` to move through your inbox, `R` to reply, and `⌘↩` to send.

4AM is a small menu bar app that gives Apple Mail the single-key shortcuts Gmail users miss. Apple Mail's own shortcuts all need a modifier key, and the old Mail plug-ins that added Gmail keys no longer work on current macOS. 4AM is a separate app that needs no plug-in.

**[Download the free trial](https://caninodigital.com/4am/4AM.dmg)** · **[Product page](https://caninodigital.com/4am/)** · **[Buy a license (USD$9.99)](https://caninodigital.lemonsqueezy.com/checkout/buy/dadbaa88-5737-48e0-9b0e-56587e397f38)**

<p align="center"><img src="assets/panel.png" width="400" alt="The 4AM menu bar panel, showing switches and the list of single-key shortcuts"></p>

## Shortcuts

| Key | Action | Key | Action |
|---|---|---|---|
| `E` | Archive | `S` | Flag |
| `#` | Delete | `!` | Mark as spam |
| `J` | Next message | `⇧I` | Mark read |
| `K` | Previous message | `⇧U` | Mark unread |
| `R` | Reply | `Z` | Undo |
| `A` | Reply all | `/` | Search |
| `F` | Forward | `O` or `↩` | Open message |
| `C` | New message | `⌘↩` | Send (in a compose window) |

They work in the message list and in a message opened in its own window. Every key can be changed or switched off.

## Install

1. Download [4AM.dmg](https://caninodigital.com/4am/4AM.dmg), open it and drag 4AM into Applications. Open 4AM.
2. macOS asks to let 4AM control your Mac. Choose **Open System Settings** and switch 4AM on. If it isn't in the list, add it with the **+** button.
3. In Mail, select a message and press a key. Click the 4AM icon in the menu bar to see every shortcut.

Requires **macOS 27 or later**. The download is signed and notarised by Apple.

## Privacy

An app that listens for keys has to earn trust, so here is exactly what 4AM does:

- **It never records what you type.** Each key is checked against your shortcut list and forgotten. Nothing is logged or stored.
- **It only looks at the keyboard while Mail is in front.** Switch to another app and it stops entirely.
- **Typing is never touched.** Shortcuts fire only when a message or the message list is selected. Writing an email, searching and Spotlight work as normal.
- **One network connection, when you ask.** 4AM contacts the internet only when you activate or deactivate a license key, sending that key and your Mac's name. Nothing about your mail is ever sent.

## What 4AM needs access to

| Access | Why | What it doesn't do |
|---|---|---|
| **Accessibility** (required) | To see which part of Mail is selected, notice shortcut keys while Mail is in front, and press Mail's own menu commands, such as Archive, for you. | It doesn't read the content of your emails. It looks at what kind of element is selected (for example "the message list"), not what's in it. It does read the names of Mail's menu items, which is how it finds commands such as Archive. |
| **Input Monitoring** (only if macOS asks) | On some setups macOS wants this as well before an app can notice key presses. 4AM asks only if it's needed on your Mac. | Same as above: keys are checked against your shortcut list and forgotten. |
| **Internet** (only when you activate) | To confirm a license key with Lemon Squeezy, sending the key and your Mac's name. | No analytics, no tracking, no update checks, and nothing about your mail. |
| **Keychain** | To store your license key and the date your trial started. The trial date is kept there on purpose so that deleting and reinstalling the app doesn't restart the trial; it stays until you remove it (see below). | It doesn't read any of your other Keychain items. |
| **Open at login** (optional) | So 4AM starts with your Mac. It asks once; you can change it any time. | |

### What Canino Digital can see

- **When you buy:** the name and email address you give at checkout, through Lemon Squeezy, which processes the payment. Card details go to Lemon Squeezy and are never seen by Canino Digital.
- **When you activate:** the name of the Mac, such as "Sam's MacBook Air", listed against your license key so you can tell your activations apart.
- **Nothing else.** 4AM has no analytics and sends no usage data, so there is no record of how, when or whether you use it.

### Files and debugging tools

4AM keeps these on your Mac:

- `~/Library/Application Support/4AM/keymap.json`: your shortcut settings.
- `~/Library/Preferences/com.caninodigital.4AM.plist`: whether shortcuts are switched on, and similar settings.
- `~/Library/Logs/4AM/debug.log`: written only when you use the debugging tools.

The debugging tools appear when you hold Option and click the menu bar icon. They exist to diagnose problems after a macOS update. They record which shortcut ran and the kind of element selected in Mail, never the keys you press or any text. One tool, "Log Menu Structure", writes the names of Mail's menus to that log, which can include your mailbox names. The log stays on your Mac and is never sent anywhere; you choose whether to share it when reporting a problem.

### Removing 4AM completely

1. Quit 4AM and delete it from Applications.
2. Remove it under System Settings › Privacy & Security (Accessibility, and Input Monitoring if listed) and under General › Login Items.
3. Delete the three files listed above.
4. In the Keychain Access app, search for `com.caninodigital.4AM.license` and delete the entries. These hold your license key and trial date.

## Pricing

Free for 7 days with everything working. After that, a one-time purchase of USD$9.99 unlocks it. No subscription. A license key works on up to 3 Macs and can be moved by choosing **Deactivate on This Mac**.

## Questions

**Can Apple Mail use Gmail keyboard shortcuts?**
Not by itself. 4AM adds them.

**How do I archive in Apple Mail with one key?**
With 4AM, select a message and press `E`. Without it, Mail's archive shortcut is Control-Command-A.

**Does it work with Gmail, iCloud and Outlook accounts?**
4AM works with Apple Mail itself, so it should work with any account you've added to Mail. Try the free trial to check it with yours.

**Will it keep working after macOS updates?**
4AM is tested on macOS 27 with Mail 16. It relies on parts of macOS that Apple can change at any time, so compatibility with future macOS versions isn't guaranteed. Fixes are released when possible.

## Support

- **Found a bug or have a request?** [Open an issue](../../issues).
- **Anything else:** 4am@caninodigital.com

## About this repository

This repository holds 4AM's documentation, release notes and issue tracker. 4AM is not open source and its source code is not published here.

4AM is made by [Canino Digital](https://caninodigital.com/). It is an independent app and is not affiliated with or endorsed by Apple or Google. Apple Mail and macOS are trademarks of Apple Inc. Gmail is a trademark of Google LLC.

© 2026 John Canino. All rights reserved.
