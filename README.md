# <img src="https://raw.githubusercontent.com/alexyushkin/ringkeeper/main/web/public/icon-192.png" alt="" width="40" align="top"> Ringkeeper

Ringkeeper lets one person run AI agents across many clients without ever
switching connections.

If you work for 100 clients, each has its own database, Airtable, Vercel, n8n
and email. With Claude Desktop or Claude Code you reconnect your tools every
time you switch clients. In Ringkeeper you connect each client's tools once,
attach them to that client's projects, and forget about it.

Then just ask: "Add last week's leads to Acme's Airtable." Ringkeeper figures
out which client and project you mean, uses that project's connections, and
picks the right model for the job.

- Connect once per client, use in every project that needs it
- Requests go to the right project automatically
- One client's connections can never reach another client's project
- Changes to live data wait for your approval; everything is logged
- Runs on your own computer, with your own Claude API key

Free and open source (MIT). Windows. Beta.

This repository holds the installers and update files only.

## Download

**[Download the latest release](https://github.com/alexyushkin/ringkeeper-releases/releases/latest)**
and run `Ringkeeper_<version>_x64-setup.exe` (Windows 10 and 11).

It installs for your user only: no administrator rights, nothing else to
install, no terminal. Ringkeeper opens when it's done and walks you through
first run; you need an Anthropic API key
([platform.claude.com](https://platform.claude.com) → API keys). Installed apps
update themselves from the releases here.

**Windows may warn you first.** Until the installer is signed and well known,
Microsoft Defender SmartScreen shows **"Windows protected your PC"**. Click
**More info**, check that the app is `Ringkeeper_..._x64-setup.exe`, then
click **Run anyway**. (If your browser flags the download, choose **Keep**.)
If instead **Smart App Control** blocks it (some new Windows 11 PCs have it
on), there's no "Run anyway": use a signed release once there is one.
Turning Smart App Control off is possible in Windows Security, but it can't be
turned back on without reinstalling Windows.

## Mac, experimental

**Experimental and unsigned: reports welcome.**
Each release also has two Mac downloads, for macOS 12 or newer. To see which
is yours, open the Apple menu › **About This Mac**:

- **Chip: Apple M1** or newer: `Ringkeeper_<version>_aarch64.dmg`
- **Processor: Intel**: `Ringkeeper_<version>_x64.dmg`

1. Download the `.dmg` from the
   [latest release](https://github.com/alexyushkin/ringkeeper-releases/releases/latest),
   open it, and drag **Ringkeeper** into **Applications**.
2. **Don't double-click it the first time:** the app isn't signed yet, so macOS
   won't open it that way. In Finder, choose **Go › Applications** from the menu
   bar, right-click **Ringkeeper** (or hold Control and click it), and choose
   **Open**.
3. macOS asks if you're sure. Click **Open**. It remembers this, so you only do
   it once.

If that message has no **Open** button (macOS 15 or newer), click **Done**. Then
open **System Settings › Privacy & Security**, scroll down to **Security**, and
next to "Ringkeeper was blocked…" click **Open Anyway**. Confirm with your
password or Touch ID, then click **Open**.

If macOS instead says the app "is damaged and can't be opened", that's the same
missing signature. In Terminal, run
`xattr -dr com.apple.quarantine /Applications/Ringkeeper.app`, then open it
again.

Your data goes in `~/Library/Application Support/Ringkeeper`, the master key in
your Keychain, and new projects in `Documents/Ringkeeper`. Updates install from
inside the app, as on Windows.

Something not working on your Mac? Please
[open an issue](https://github.com/alexyushkin/ringkeeper-releases/issues):
that's how the Mac build gets tested.

## Problems

[Open an issue](https://github.com/alexyushkin/ringkeeper-releases/issues) with
what you did, what happened, and your Windows version. Ringkeeper's version is
in Settings › About.

## Need help setting it up?

I can help you install and connect Ringkeeper for your clients. Contact:
<https://yushkin.us> or LinkedIn: <https://www.linkedin.com/in/alexey-yushkin>.

## License

MIT, see [LICENSE](LICENSE). The installers also contain third-party software
under its own licenses, listed in the app under Settings › About.
