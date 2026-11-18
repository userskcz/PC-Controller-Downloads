# PC Controller — Windows Server

Сервер для керування ПК із годинника Wear OS. / Windows companion for the PC Controller Wear OS app.

## Завантаження / Download

**[Завантажити сервер для Windows / Download Windows Server](https://github.com/userskcz/PC-Controller-Downloads/releases/download/v1.6.31-rc.1/PC-Server-Setup.exe)**

Windows x64 · версія / version **1.6.31** · попередній випуск / **pre-release** · EXE **158,904,241 bytes**.

[Опис випуску та SHA-256 / Release notes and SHA-256](https://github.com/userskcz/PC-Controller-Downloads/releases/tag/v1.6.31-rc.1) · [Усі версії / All releases](https://github.com/userskcz/PC-Controller-Downloads/releases)

## Підключення годинника

1. Завантажте `PC-Server-Setup.exe` на ПК із Windows, установіть і запустіть **PC Server**.
2. Під’єднайте ПК і годинник до мережі, у якій годинник має доступ до ПК. За потреби дозвольте PC Server у брандмауері Windows для приватної мережі.
3. Відкрийте адресу сервера й API-ключ у PC Server. У застосунку годинника відкрийте **Settings**, введіть **PC URL** та **API Key**, натисніть **Test PC**.
4. Після успішного підключення перевірте керування музикою чи гучністю.

Застосунок на годиннику встановлюється окремо. Застосунок-компаньйон на телефоні не потрібен. Для зовнішнього доступу використовуйте захищене HTTPS/VPN-з’єднання. Звичайний локальний HTTP не зашифрований. Не відкривайте сервер напряму в інтернет без належного захисту.

Wake-on-LAN залежить від обладнання й налаштувань ПК. Для камер можуть знадобитися права адміністратора. Presence/Unlock потребує окремого налаштування компонентів Windows та Bluetooth. У цьому попередньому випуску перевірка фізичного Bluetooth, Sleep/Resume та наскрізного Unlock ще не завершена.

## Connect your watch

1. Download `PC-Server-Setup.exe` on your Windows PC, install it and start **PC Server**.
2. Connect the watch and PC through a reachable network. If needed, allow PC Server through Windows Firewall on your private network.
3. Find the server address and API key in PC Server. On your watch, open **Settings**, enter **PC URL** and **API Key**, then select **Test PC**.
4. After connecting, test media or volume controls.

The watch app is installed separately. No phone companion app is required. Use secured HTTPS/VPN for remote access; local HTTP traffic is unencrypted. Do not expose the server directly to the internet without appropriate protection.

Wake-on-LAN requires compatible hardware and configuration. Camera control may require administrator rights. Presence/Unlock requires separate Windows and Bluetooth setup. Physical Bluetooth, Sleep/Resume and complete Unlock testing are still pending for this pre-release.

## Перевірка файлу / Verify your download

SHA-256 для / for `PC-Server-Setup.exe`:

```text
53b296cc9c78bea94dadc6e54560e5a5e3827acbff79e2ab068cc4e0c4313302
```

PowerShell:

```powershell
Get-FileHash -LiteralPath .\PC-Server-Setup.exe -Algorithm SHA256
```

Інсталятор не має підпису Authenticode. Windows може показати попередження про невідомого видавця. Перевірте джерело та SHA-256; не вимикайте захист Windows.

The installer is not Authenticode signed. Windows may display an unknown-publisher warning. Verify the source and SHA-256; do not disable Windows protection.

## Підтримка / Support

[Повідомити про проблему / Report an issue](https://github.com/userskcz/PC-Controller-Downloads/issues/new/choose)

Додайте версію сервера, модель годинника, версію Wear OS та кроки відтворення. Не публікуйте API-ключі, токени, паролі чи приватні файли. / Include the server version, watch model, Wear OS version and reproduction steps. Do not post API keys, tokens, passwords or private files.

Цей репозиторій містить інсталятори й документацію. Вихідний код зберігається окремо й не публікується тут. / This repository distributes installers and documentation. Application source code is maintained separately and is not published here.

[Умови використання / Terms](TERMS.md)
