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

## Problems

[Open an issue](https://github.com/alexyushkin/ringkeeper-releases/issues) with
what you did, what happened, and your Windows version. Ringkeeper's version is
in Settings › About.

## License

MIT, see [LICENSE](LICENSE). The installers also contain third-party software
under its own licenses, listed in the app under Settings › About.
