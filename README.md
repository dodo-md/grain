# grain

A minimal macOS application built with Swift 6 and AppKit.

## Development

Open `Grain.xcodeproj`, select the `Grain` scheme, and run.

Build from the command line:

```sh
xcodebuild -project Grain.xcodeproj -scheme Grain -configuration Debug -derivedDataPath build build
```

Use `-configuration Release` for an optimized build.

The application currently only starts the AppKit event loop. It intentionally has no window, menu, or editor UI until the design is approved. Stop it using Xcode's Stop button.

## Project scope

- One application target and one Swift source file, with no external dependencies.
- Swift Package Manager is reserved for modularization with a clear benefit.
- Local builds use ad-hoc signing and the placeholder bundle identifier `local.grain.Grain`.
- The deployment target inherits the selected macOS SDK default. A minimum supported macOS version and distribution signing are not decided yet.
