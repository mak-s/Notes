# Whats new in Xcode 15
## WWDC 2023
[What's new in Xcode 15 - WWDC23][What's new in Xcode 15]

---
- Editing
  - Code completion updates
  - What's new in asset catalogs
  - Meet string catalogs
  - What's new in Swift-DocC
  - Meet Swift macros
  - What's new in Previews
- Navigating
  - The bookmark navigator
- Sharing
  - What's new in source control
- Testing
  - What's new in testing
- Debugging
  - Updates in the debug console
- Distribution
  - Updates in Xcode Cloud distribution
  - Signature verification and privacy manifests
  - What's new in Xcode distribution

---

## Code completion updates

- when creating a class/struct in a new file, the file name is suggested as class/struct name
- pressing right arrow key shows all possible permutation of a method with multiple default arguments.
- pressing a `.` to add additional modifiers to a view, shows the most frequently used modifier.
- adding another modifier to the view, does not suggest already added modifier.

---

## What's new in asset catalogs

- colors and images in asset catalog are backed by swift symbols.
e.g an image named `clouds` can be accessed using `.clouds`

---

## Meet string catalogs

Migrate all your string localization to String catalog
For more see: [Discover String Catalog][Discover String catalog]

---

## What's new in Swift-DocC

- new styling and spacing
- new Documentation assistant (Editor > Assistant > Documentation preview)
For more see: [Create rich documentation with Swift-DocC][Create rich documentation with Swift-DocC]
---

## Meet Swift macros
- inbuilt macros for `@Observable`, `#Predicate`, `@Model`.
- write custom Macros using Macro package

For more, see:
- [Expand on Swift macros][Expand on Swift Macros]
- [Write Swift macros][Write Swift Macros]

---

## What's new in Previews
- inbuilt macro `#Preview`
- preview available for UIKit and AppKit apps.
- previews for Widgets

For more, see [Build programmatic UI with Xcode Previews][Build programmatic UI with Xcode previews]

---

## The bookmark navigator

---

## What's new in source control

---

## What's new in testing

See: [Fix failures faster with Xcode test reports][Fix failures faster with Xcode test reports]

---

## Updates in the debug console

See: [Debug with structured logging][Debug with structured logging]

---

## Updates in Xcode Cloud distribution

---

## Signature verification and privacy manifests

See: 
- [Verify app dependencies with digital signature][Verify app dependencies with digital signature]
- [Get started with privacy manifest][Get started with privacy manifest]

---

## What's new in Xcode distribution

See [Simplify distribution in Xcode and Xcode Cloud - WWDC23][Simplify distribution in Xcode and Xcode Cloud]

---

## Reference

- [What's new in Xcode 15 - WWDC23][What's new in Xcode 15]
- [Discover String Catalog - WWDC23][Discover String catalog]
- [Create rich documentation with Swift-DocC - WWDC23][Create rich documentation with Swift-DocC]
- [Expand on Swift macros - WWDC23][Expand on Swift Macros]
- [Write Swift macros - WWDC23][Write Swift Macros]
- [Build programmatic UI with Xcode previews - WWDC23][Build programmatic UI with Xcode previews]
- [Fix failures faster with Xcode test reports - WWDC23][Fix failures faster with Xcode test reports]
- [Debug with structured logging - WWDC23][Debug with structured logging]
- [Verify app dependencies with digital signature - WWDC23][Verify app dependencies with digital signature]
- [Get started with privacy manifest - WWDC23][Get started with privacy manifest]
- [Simplify distribution in Xcode and Xcode Cloud - WWDC23][Simplify distribution in Xcode and Xcode Cloud]


[What's new in Xcode 15]: https://developer.apple.com/videos/play/wwdc2023/10165/
[Discover String catalog]: https://developer.apple.com/videos/play/wwdc2023/10155
[Create rich documentation with Swift-DocC]: https://developer.apple.com/videos/play/wwdc2023/10244
[Expand on Swift Macros]: https://developer.apple.com/videos/play/wwdc2023/10167
[Write Swift Macros]: https://developer.apple.com/videos/play/wwdc2023/10166
[Build programmatic UI with Xcode previews]: https://developer.apple.com/videos/play/wwdc2023/10252
[Fix failures faster with Xcode test reports]: https://developer.apple.com/videos/play/wwdc2023/10175
[Debug with structured logging]: https://developer.apple.com/videos/play/wwdc2023/10226
[Verify app dependencies with digital signature]: https://developer.apple.com/videos/play/wwdc2023/10061
[Get started with privacy manifest]: https://developer.apple.com/videos/play/wwdc2023/10060
[Simplify distribution in Xcode and Xcode Cloud]: https://developer.apple.com/videos/play/wwdc2023/10224
