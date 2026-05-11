# Cursor Work Profile

This guide shows how to open a separate Cursor profile named `Cursor_Work` on Windows and macOS.

Using a separate profile lets you sign in with a different Cursor account, keep extensions separate, and isolate settings from your main Cursor profile.

## Windows

Run this from Command Prompt, PowerShell, or a Windows shortcut target:

```bat
C:\Users\fl-sayyid.khan\AppData\Local\Programs\cursor\Cursor.exe --user-data-dir="C:\Users\fl-sayyid.khan\Cursor_Work"
```

If your Windows username is different, change both paths to match your actual user folder.

Example:

```bat
C:\Users\YOUR_USERNAME\AppData\Local\Programs\cursor\Cursor.exe --user-data-dir="C:\Users\YOUR_USERNAME\Cursor_Work"
```

## macOS Terminal Alias

The macOS equivalent command is:

```bash
/Applications/Cursor.app/Contents/MacOS/Cursor --user-data-dir="$HOME/Cursor_Work"
```

To make it easier to run, add this alias to `~/.zshrc`:

```bash
alias cursor-work='/Applications/Cursor.app/Contents/MacOS/Cursor --user-data-dir="$HOME/Cursor_Work"'
```

Reload your shell config:

```bash
source ~/.zshrc
```

Then open Cursor Work from Terminal:

```bash
cursor-work
```

## macOS Clickable App Shortcut

The clickable shortcut created on this Mac lives here:

```text
/Users/sayyid/Applications/Cursor Work.app
```

You can open it with Spotlight:

1. Press `Cmd + Space`
2. Type `Cursor Work`
3. Press `Enter`

## Profile Folder Locations

Windows profile folder:

```text
C:\Users\fl-sayyid.khan\Cursor_Work
```

macOS profile folder:

```text
/Users/sayyid/Cursor_Work
```

## Notes

- Close Cursor completely before opening another profile if Cursor reuses the existing window.
- Use a different `--user-data-dir` value for each separate account.
- The profile folder is created automatically the first time you launch Cursor with that path.
