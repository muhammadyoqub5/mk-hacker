# mk-hacker
LOCWATCHER TOOL FOR LINUX
**Lockwatcher_ultimate** is a powerful Linux terminal security monitoring tool written in pure Bash. It watches for unauthorized or suspicious `sudo`, `su`, and `passwd` attempts and immediately sends alerts via Telegram, email, desktop notifications, and logs the activity in CSV format.

It is designed for cybersecurity enthusiasts, system administrators, and penetration testers to help detect privilege escalation attempts and maintain terminal-level visibility in real-time.

---

## 🔍 Features

- 🧠 Detects `sudo`, `su`, and `passwd` usage in real-time
- 📲 Sends alerts to Telegram (bot API)
- 📧 Sends email alerts (via mail/sendmail)
- 🖥️ Desktop notifications using `notify-send`
- 📊 CSV logging for later analysis (timestamp, user, tty, IP, command)
- 📟 Interactive terminal GUI using `dialog`
- 🔁 Real-time log file monitoring via `inotify-tools`
- 🚀 Can be configured to run as a `systemd` service
- 🌐 Remote server monitoring via SSH (optional)

---

## ⚙️ Requirements

- Bash shell
- `curl`, `mailutils`, `notify-send`, `dialog`, `inotify-tools`
- A Telegram bot token and chat ID
- Optional: email configured via `mailx` or `sendmail`

Install dependencies:

```bash
sudo apt update
sudo apt install curl mailutils libnotify-bin dialog inotify-tools -y
