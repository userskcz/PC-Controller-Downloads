# PC Controller — Windows Server

Windows companion for the PC Controller Wear OS app.

## Download

**[Download Windows Server](https://github.com/userskcz/PC-Controller-Downloads/releases/download/v1.6.31-rc.1/PC-Server-Setup.exe)**

Windows x64 · version **1.6.31** · **pre-release** · EXE **158,904,241 bytes**.

[Release notes and SHA-256](https://github.com/userskcz/PC-Controller-Downloads/releases/tag/v1.6.31-rc.1) · [All releases](https://github.com/userskcz/PC-Controller-Downloads/releases)

## Connect your watch

1. Download `PC-Server-Setup.exe` on your Windows PC, install it and start **PC Server**.
2. Connect the watch and PC through a reachable network. If needed, allow PC Server through Windows Firewall on your private network.
3. Find the server address and API key in PC Server. On your watch, open **Settings**, enter **PC URL** and **API Key**, then select **Test PC**.
4. After connecting, test media or volume controls.

The watch app is installed separately. No phone companion app is required. Use secured HTTPS/VPN for remote access; local HTTP traffic is unencrypted. Do not expose the server directly to the internet without appropriate protection.

Wake-on-LAN requires compatible hardware and configuration. Camera control may require administrator rights. Presence/Unlock requires separate Windows and Bluetooth setup. Physical Bluetooth, Sleep/Resume and complete Unlock testing are still pending for this pre-release.

## Verify your download

SHA-256 for `PC-Server-Setup.exe`:

```text
53b296cc9c78bea94dadc6e54560e5a5e3827acbff79e2ab068cc4e0c4313302
```

PowerShell:

```powershell
Get-FileHash -LiteralPath .\PC-Server-Setup.exe -Algorithm SHA256
```

The installer is not Authenticode signed. Windows may display an unknown-publisher warning. Verify the source and SHA-256; do not disable Windows protection.

## Support

[Report an issue](https://github.com/userskcz/PC-Controller-Downloads/issues/new/choose)

Include the server version, watch model, Wear OS version and reproduction steps. Do not post API keys, tokens, passwords or private files.

This repository distributes installers and documentation. Application source code is maintained separately and is not published here.

[Terms](TERMS.md)
