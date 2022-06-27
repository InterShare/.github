## InterShare

InterShare aims to be a cross platform open source AirDrop alternative, enabling you to send files with ease to other devices over the local network.

## Status 

While it works, currently it may not be well-designed to be used by anyone other than my colleges. 

<b>Feature list</b>
- ✅ Transfer (TCP)
- ✅ Discovery (UDP + MDNS)
- ✅ App for Linux, macOS, Windows, iOS and Android
- ✅ Encryption
- ⏳ Rewrite in Rust
- ⏳ Native apps per platform
- 🗓 Authentication (via ECDSA probably)
- 🗓 Publish linux package (AppImage, rpm and deb)
- 🗓 Bluetooth discovery and transfer

✅ = Done and published <br />
⏳ = Working on it  <br />
🗓 = Planned <br />

## How it currently works

Currently the SMTS-Protocol, which is used to transfer the data, is implemented in C#.

## How it will work in the future

While InterShare currently works as C# .NET Application. It is only temporary. The plan is to rewrite the SMTS-Protocol in Rust and use the FFI to write native apps per platform.

- Swift for macOS, iOS
- Rust as GTK App for Linux
- .NET WinUI 3 App for Windows
- Either Kotlin or Xamarin.Android for Android.

