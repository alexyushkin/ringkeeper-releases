# Ringkeeper

Ringkeeper runs Claude coding agents on your own computer, against the projects
and accounts you give them. Each project is bound to its own connections (its
Supabase, its n8n, its Vercel team), so an agent working on one client can't
reach another's. Writes to production wait for your approval, and everything is
recorded in an audit log. It is MIT licensed and in beta.

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
