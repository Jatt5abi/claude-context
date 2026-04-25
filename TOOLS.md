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

## Keyboard Shortcuts — Aula S99 Pro (updated 2026-04-24, via gsettings)
- **F7** — Previous track
- **F8** — Play/Pause
- **F9** — Next track
- **F10** — Mute
- **F11** — Volume down
- **F12** — Volume up
- Note: input-remapper not needed — gsettings binds F7-F12 directly

## Audio
- Speakers: Pioneer passive bookshelf (left tweeter blown — needs replacement)
- Amp: Facmogu F900S 160W BT5.0 — paired to Mac via Bluetooth
- EQ: EasyEffects installed (`sudo apt install easyeffects`)

## Useful Commands
```bash
# Media keys gsettings (Aula S99 Pro)
gsettings set org.gnome.settings-daemon.plugins.media-keys previous "['F7']"
gsettings set org.gnome.settings-daemon.plugins.media-keys play "['F8']"
gsettings set org.gnome.settings-daemon.plugins.media-keys next "['F9']"
gsettings set org.gnome.settings-daemon.plugins.media-keys volume-mute "['F10']"
gsettings set org.gnome.settings-daemon.plugins.media-keys volume-down "['F11']"
gsettings set org.gnome.settings-daemon.plugins.media-keys volume-up "['F12']"

# Package install pattern
sudo apt install <package>

# Snap install pattern  
sudo snap install <package>
```
