# TOOLS.md — Mac Mini Setup & Commands

## scrcpy — Phone Mirror to Linux
- Working binary: `~/scrcpy-linux-x86_64-v3.3.1/scrcpy`
- Snap version broken (gpu-2404 slot issue) — never use `/snap/bin/scrcpy`
- **Wired (USB):** `~/scrcpy-linux-x86_64-v3.3.1/scrcpy -d` (requires USB File Transfer / MTP mode)
- **Wireless:** `adb connect IP:PORT` → `~/scrcpy-linux-x86_64-v3.3.1/scrcpy --tcpip=IP:PORT`
- Wireless port changes every time you leave/re-enter Wireless Debugging on phone
- Mouse scroll wheel = swipe up/down in TikTok
- Clipboard sync phone→Mac works; Mac→phone needs `--clipboard-autosync` flag

## File Transfer Phone ↔ Mac
- **LocalSend** (snap) — works, requires IP/PIN on same WiFi
- **Google Drive 5TB** — fallback

## Bluetooth Fix (2026-04-18)
- BCM UART Bluetooth was failing
- Fixed: `sudo apt install apple-firmware-script` → `sudo get-apple-firmware` (option 3) → full reboot

## Keyboard Shortcuts (mapped 2026-04-20)
- **F1** — Open Spotify
- **F2** — Volume down
- **F3** — Volume up
- **F4** — Mute
- **F5** — Stop
- **F6** — Previous track
- **F7** — Play/Pause
- **F8** — Next track

## Audio
- Speakers: Pioneer passive bookshelf (left tweeter blown — needs replacement)
- Amp: Facmogu F900S 160W BT5.0 — paired to Mac via Bluetooth
- EQ: EasyEffects installed (`sudo apt install easyeffects`)

## Useful Commands
```bash
# Spotify shortcut gsettings
gsettings set org.gnome.settings-daemon.plugins.media-keys volume-down "['F2']"

# Package install pattern
sudo apt install <package>

# Snap install pattern  
sudo snap install <package>
```
