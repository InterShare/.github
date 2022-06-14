## InterShare

InterShare aims to be a cross platform open source AirDrop alternative, enabling you to send files with ease to other devices over the local network.

## Status 

While it works, currently it may not be well-designed to be used by anyone other than my colleges. 

<b>Feature list</b>
- ✅ Transfer (TCP)
- ✅ Discovery (UDP + MDNS)
- ✅ App for Linux, macOS, Windows, iOS and Android
- ✅ Encryption
- ⏳ Native apps per platform
- 🗓 Authentication (via ECDSA probably)
- 🗓 Publish linux package (AppImage, rpm and deb)

✅ = Done <br />
⏳ = Working on it  <br />
🗓 = Planned <br />

## How it currently works

Currently the SMTS-Protocol, which is used to transfer the data, is implemented in C#.

The desktop program for Linux, macOS and Windows is written in C# with the Eto.Forms GUI library. Since the library doesn't have the best documentation, many things in this project are a bit hacky. Mostly because I don't know any better. I originally wanted to program the GUI in xaml as well (which Eto.Forms actually supports), but since there is almost no documentation for it and I couldn't figure out necessary parts like bindings, I decided against it.

So with all these problems, why did I choose Eto.Forms?

I am a big fan of a native GUI experience per platform. Eto is cross-platform and uses the native GUI widgets per platform, and I couldn't find any other library that could do that. (At the time of writing .NET MAUI was still very unstable and without Linux support).


## How it will work in the future

While InterShare currently works as C# .NET Application. It is only temporary. The plan is to rewrite the SMTS-Protocol in Rust and use FFI wrapper, to write native apps per platform.

- Swift for macOS, iOS
- Rust as GTK App for Linux
- .NET WinUI 3 App for Windows
- Either Kotlin or Xamarin.Android for Android.

