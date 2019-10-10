# Surge has been moved to its own organization on GitHub

The Surge project is now located at [@Jounce/Surge](https://github.com/Jounce/Surge).

## Updating Your Dependencies

For compatibility,
an archived copy of Surge will be hosted at @mattt/Surge for some time.
If your project uses Surge,
please update your dependency to point to @Jounce/Surge.

Specific instructions for Swift Package Manager, CocoaPods, and Carthage
can be found below:

### Swift Package Manager

In `Package.swift`,
update the `url` value in your Surge `.package` declaration
in your project dependencies:

```swift
let package = Package(
    name: "myproject",
    dependencies: [
        .package(url: "https://github.com/Jounce/Surge.git", .upToNextMajor(from: "2.0.0")),
    ],
    targets: [
        .target(
            name: "myproject",
            dependencies: ["Surge"]),
    ]
)
```

### CocoaPods

**No changes are necessary.**
You can continue to use the `Surge` pod without any problem.

```ruby
pod 'Surge', '~> 2.0.0'
```

### Carthage

Update your Surge dependency declaration to the following:

```ruby
github "Jounce/Surge" ~> 2.0.0
```
