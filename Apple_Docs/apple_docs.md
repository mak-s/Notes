# Release Notes

| Title | <div style="width:290px">Description</div> | URL |
| --- | --- | --- |
| iOS & iPadOS Release Notes | Learn about changes to the iOS & iPadOS SDK. | https://developer.apple.com/documentation/ios-ipados-release-notes |
| macOS Release Notes | Learn about changes to the macOS SDK. | https://developer.apple.com/documentation/macos-release-notes |
| Safari Release Notes | Learn about changes for Safari and Safari View Controller for iOS, iPadOS, macOS, and in visionOS; WKWebView for iOS, iPadOS, macOS, watchOS, and in visionOS; and Web Inspector on macOS. | https://developer.apple.com/documentation/safari-release-notes |
| Updates | View major documentation updates and highlights from WWDC, browse ongoing updates from a set of framework releases over time, and jump to the latest release notes. | https://developer.apple.com/documentation/Updates |
| Technotes | Learn about specific development topics through these in-depth technical articles. | https://developer.apple.com/documentation/Technotes |
| tvOS Release Notes | Learn about changes to the tvOS SDK. | https://developer.apple.com/documentation/tvos-release-notes |
| visionOS Release Notes | Learn about changes to the visionOS SDK. | https://developer.apple.com/documentation/visionos-release-notes |
| watchOS Release Notes | Learn about changes to the watchOS SDK. | https://developer.apple.com/documentation/watchos-release-notes |
| Xcode Release Notes | Learn about changes to Xcode. | https://developer.apple.com/documentation/Xcode-Release-Notes |
| SwiftUI Updates | Learn about important changes to SwiftUI. | https://developer.apple.com/documentation/Updates/SwiftUI |


# Frameworks

| Framework | <div style="width:290px">Description</div> | iOS | iPadOS | Mac Catalyst | macOS | tvOS | visionOS | watchOS | Swift Playgrounds | Swift | Xcode | <div style="width:290px">NOTE</div> |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Accelerate | Make large-scale mathematical computations and image calculations, optimized for high performance and low energy consumption. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 13.1+ | macOS 10.3+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Accessibility | Make your apps accessible to everyone who uses Apple devices. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ | tvOS 14.0+ | visionOS 1.0+ | watchOS 7.0+ |  |  |  |  |
| AccessorySetupKit | Enable privacy-preserving discovery and configuration of accessories. | iOS 18.0+ | iPadOS 18.0+ |  |  |  |  |  |  |  |  | AccessorySetupKit is available for iOS and iPadOS. In watchOS 26 and later, if someone sets up an accessory with your iOS app by using AccessorySetupKit, a companion watchOS app can also use CoreBluetooth to communicate with the new accessory and any other accessories. |
| AccessoryTransportExtension-Beta | Exchange sensitive information with a connected accessory. | iOS 26.2+Beta | iPadOS 26.2+Beta | Mac Catalyst 26.2+Beta |  |  |  |  |  |  |  | The Accessory Transport Extension framework is available for iOS. For apps built with Catalyst for macOS, and for iOS apps running on visionOS or on Mac computers with Apple silicon, calls to the framework do nothing. |
| ActivityKit | Share live updates from your app as Live Activities on iPhone, iPad, Apple Watch, and the Mac. | iOS 16.1+ | iPadOS 16.1+ |  |  |  |  |  |  |  |  |  |
| AdAttributionKit | Present, process, and register postbacks for in-app ads in the App Store and alternative app marketplaces. | iOS 17.4+ | iPadOS 17.4+ | Mac Catalyst 17.4+ |  |  |  |  |  |  |  |  |
| Address Book | Access the centralized database for storing users’ contacts. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 14.0+ | macOS 10.2+ |  |  |  |  |  |  | Do not use the AddressBook framework in macOS 10.11 and later. Use the APIs defined in the Contacts framework instead. |
| Address Book UI | Access users’ contacts and display them in a graphical interface. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 14.0+ |  |  |  |  |  |  |  | Do not use the AddressBookUI framework in iOS 9 and later. Use the APIs defined in the Contacts UI framework instead. |
| AdServices | Attribute app-download campaigns that originate from the App Store on iOS devices. | iOS 14.3+ | iPadOS 14.3+ | Mac Catalyst 14.3+ | macOS 11.1+ |  | visionOS 1.0+ |  |  |  |  |  |
| AdSupport | Provide apps with access to an advertising identifier. | iOS 6.0+ | iPadOS 6.0+ | Mac Catalyst 13.0+ | macOS 10.14+ | tvOS 9.0+ |  |  |  |  |  |  |
| AlarmKit | Schedule prominent alarms and countdowns to help people manage their time. | iOS 26.0+ | iPadOS 26.0+ |  |  |  |  |  |  |  |  |  |
| App Clips | Create a lightweight, in-the-moment experience or demo version for your app that’s instantly available. | iOS 14.0+ | iPadOS 14.0+ |  |  |  |  |  |  |  |  |  |
| App Intents | Make your app’s content and actions discoverable with system experiences like Spotlight, widgets, and the Shortcuts app. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| App Tracking Transparency | Request user authorization to access app-related data for tracking the user or the device. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ | tvOS 14.0+ | visionOS 1.0+ |  |  |  |  |  |
| AppKit | Construct and manage a graphical, event-driven user interface for your macOS app. |  |  | Mac Catalyst 13.0+ | macOS 10.0+ |  |  |  |  |  |  |  |
| Apple Archive | Perform multithreaded lossless compression of directories, files, and data. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ | tvOS 14.0+ | visionOS 1.0+ | watchOS 7.0+ |  |  |  |  |
| Apple CryptoKit | Perform cryptographic operations securely and efficiently. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 15.0+ | macOS 10.15+ | tvOS 15.0+ | visionOS 1.0+ | watchOS 8.0+ |  |  |  |  |
| Application Services | Perform common application tasks. |  |  | Mac Catalyst 13.0+ | macOS 10.0+ |  |  |  |  |  |  |  |
| AppMigrationKit | Perform a one-time transfer of your app’s on-device data to or from a device running another platform. | iOS 26.1+ | iPadOS 26.1+ |  |  |  |  |  |  |  |  |  |
| ARKit | Integrate hardware sensing features to produce augmented reality apps and games. | iOS 11.0+ | iPadOS 11.0+ | Mac Catalyst 14.0+ |  |  | visionOS 1.0+ |  |  |  |  |  |
| Assignables | A framework that contains wrappers for a PDF to allow creation of an assessment and student work on that assessment. | iOS 15.4+ | iPadOS 15.4+ | Mac Catalyst 15.4+ |  |  |  |  |  |  |  |  |
| Audio Toolbox | Record or play audio, convert formats, parse audio streams, and configure your audio session. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.1+ | macOS 10.0+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| Authentication Services | Make it easy for users to log into apps and services. | iOS 12.0+ | iPadOS 12.0+ | Mac Catalyst 13.0+ | macOS 10.15+ | tvOS 13.0+ | visionOS 1.0+ | watchOS 6.0+ |  |  |  |  |
| Automated Device Enrollment | Allow users of third-party MDM apps to add macOS and iOS devices to their organization. | iOS 16.1+ | iPadOS 16.1+ | Mac Catalyst 16.1+ |  |  |  |  |  |  |  |  |
| Automatic Assessment Configuration | Enter single-app mode and prevent students from accessing specific system features while taking an exam. | iOS 13.4+ | iPadOS 13.4+ | Mac Catalyst 13.4+ | macOS 10.15.4+ |  |  |  |  |  |  |  |
| Automator | Develop actions that the Automator app can load and run. View, edit, and run Automator workflows in your app. |  |  | Mac Catalyst 14.0+ | macOS 10.4+ |  |  |  |  |  |  |  |
| AVFAudio | Play, record, and process audio; configure your app’s system audio behavior. | iOS 14.5+ | iPadOS 14.5+ | Mac Catalyst 14.5+ | macOS 11.3+ | tvOS 14.5+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| AVFoundation | Work with audiovisual assets, control device cameras, process audio, and configure system audio interactions. | iOS 2.2+ | iPadOS 13.1+ | Mac Catalyst 13.1+ | macOS 10.7+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 3.0+ |  |  |  |  |
| AVKit | Create user interfaces for media playback, complete with transport controls, chapter navigation, picture-in-picture support, and display of subtitles and closed captions. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.0+ | macOS 10.9+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| AVRouting | Display custom destinations to stream media in the system route picker. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 26.0+ |  |  |  |  |  |  |
| Background Assets | Improve or eliminate the time people wait while your app downloads assets. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 18.4+ | visionOS 2.4+ |  |  |  |  |  |
| Background Tasks | Support background processing in your app by wrapping your app’s most critical work in framework-provided tasks. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.1+ |  | tvOS 13.0+ | visionOS 1.0+ |  |  |  |  |  |
| BrowserEngineCore | Integrate an alternative browser engine into your web browser app. | iOS 17.4+ | iPadOS 18.0+ |  |  |  |  |  |  |  |  |  |
| BrowserEngineKit | Create a browser that renders content using an alternative browser engine. | iOS 17.4+ | iPadOS 18.0+ |  |  |  |  |  |  |  |  |  |
| BrowserKit | Check a device’s eligibility to run alternative browser engines. | iOS 18.4+ | iPadOS 18.4+ |  |  |  |  |  |  |  |  |  |
| Bundle Resources | Resources located in an app, framework, or plugin bundle. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 2.0+ | macOS 10.0+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| CallKit | Display the system-calling UI for your app’s VoIP services, and coordinate your calling services with other apps and the system. | iOS 10.0+ | iPadOS 10.0+ | Mac Catalyst 13.0+ | macOS 13.0+ |  | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| CareKit | Create apps that help people better understand and manage their health. | iOS 13.0+ |  | Mac Catalyst 13.0+ |  |  |  | watchOS 7.0+ |  |  |  |  |
| CarKey | Access the remote keyless features of configured vehicles in the Wallet app. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ |  |  |  |  |  |  |  |  |
| CarPlay | Integrate CarPlay in apps related to audio, communication, navigation, parking, EV charging, food ordering, and more. | iOS 12.0+ | iPadOS 12.0+ | Mac Catalyst 14.0+ |  |  |  |  |  |  |  |  |
| CFNetwork | Access network services and handle changes in network configurations. Build on abstractions of network protocols to simplify tasks such as working with BSD sockets, administering HTTP and FTP servers, and managing Bonjour services. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.0+ | macOS 10.8+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| Cinematic | Integrate playback and editing of assets captured in Cinematic mode into your app. | iOS 17.0+ | iPadOS 17.0+ | macOS 14.0+ |  | tvOS 17.0+ |  |  |  |  |  |  |
| ClassKit | Enable teachers to assign activities from your app’s content and to view student progress. | iOS 11.4+ | iPadOS 11.4+ | Mac Catalyst 14.0+ | macOS 11.0+ |  | visionOS 1.0+ |  |  |  |  |  |
| ClockKit | Display app-specific data on the clock face. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ |  |  |  | watchOS 10.0+ |  |  |  |  |
| CloudKit | Store structured app and user data in iCloud containers that all users of your app can share. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.0+ | macOS 10.10+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 3.0+ |  |  |  |  |
| Collaboration | Find and access identities, that is, users and groups. Display the Identity Picker, which lets users create and select identities. |  |  |  | macOS 10.5+ |  |  |  |  |  |  |  |
| ColorSync | Reproduce colors accurately across a range of input, output, and display devices. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 13.0+ | macOS 10.13+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| Combine | Customize handling of asynchronous events by combining event-processing operators. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 10.15+ | tvOS 13.0+ | visionOS 1.0+ | watchOS 6.0+ |  |  |  |  |
| Compositor Services | Take control of the drawing environment and render your own content using Metal. |  |  |  |  |  | visionOS 1.0+ |  |  |  |  |  |
| Compression | Leverage common compression algorithms for lossless data compression. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.1+ | macOS 10.11+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| ContactProvider | Provide contacts managed by your app to the system-wide Contacts ecosystem. | iOS 18.0+ | iPadOS 18.0+ |  |  |  |  |  |  |  |  |  |
| Contacts | Access the user’s contacts, and format and localize contact information. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.0+ | macOS 10.11+ |  | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Contacts UI | Provide an interface that allows people to display information about their contacts. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.0+ | macOS 10.11+ |  | visionOS 1.0+ |  |  |  |  |  |
| Core Animation | Render, compose, and animate visual elements. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.1+ | macOS 10.3+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 11.0+ |  |  |  |  |
| Core Audio | Use the Core Audio framework to interact with device’s audio hardware. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.1+ | macOS 10.0+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 3.0+ |  |  |  |  |
| Core Audio Types | Use specialized data types to interact with audio streams, complex buffers, and audiovisual timestamps. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 10.15+ | tvOS 13.0+ | visionOS 1.0+ | watchOS 6.0+ |  |  |  |  |
| Core Bluetooth | Communicate with Bluetooth low energy and BR/EDR (“Classic”) Devices. | iOS 5.0+ | iPadOS 5.0+ | Mac Catalyst 13.0+ | macOS 10.10+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 4.0+ |  |  |  |  |
| Core Data | Persist or cache data on a single device, or sync data to multiple devices with CloudKit. | iOS 3.0+ | iPadOS 3.0+ | Mac Catalyst 13.0+ | macOS 10.4+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Core Foundation | Access low-level functions, primitive data types, and various collection types that are bridged seamlessly with the Foundation framework. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.0+ | macOS 10.0+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Core Graphics | Harness the power of Quartz technology to perform lightweight 2D rendering with high-fidelity output. Handle path-based drawing, antialiased rendering, gradients, images, color management, PDF documents, and more. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.1+ | macOS 10.8+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Core Haptics | Compose and play haptic patterns to customize your iOS app’s haptic feedback. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ |  | tvOS 14.0+ | visionOS 1.0+ |  |  |  |  |  |
| Core HID | Interact with keyboards, mice, and other human interface devices. |  |  |  | macOS 15.0+ |  |  |  |  |  |  |  |
| Core Image | Use built-in or custom filters to process still and video images. | iOS 5.0+ | iPadOS 5.0+ | Mac Catalyst 13.1+ | macOS 10.11+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| Core Location | Obtain the geographic location and orientation of a device. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.0+ | macOS 10.6+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Core Media | Represent time-based audio-visual assets with essential data types. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 13.1+ | macOS 10.7+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 6.0+ |  |  |  |  |
| Core Media I/O | Securely support custom camera devices in macOS. |  |  | Mac Catalyst 13.0+ | macOS 10.7+ |  |  |  |  |  |  |  |
| Core MIDI | Communicate with MIDI devices such as hardware keyboards and synthesizers. | iOS 4.2+ | iPadOS 4.2+ | Mac Catalyst 13.0+ | macOS 10.0+ | tvOS 15.0+ | visionOS 1.0+ | watchOS 8.0+ |  |  |  |  |
| Core ML | Integrate machine learning models into your app. | iOS 11.0+ | iPadOS 11.0+ | Mac Catalyst 13.0+ | macOS 10.13+ | tvOS 11.0+ | visionOS 1.0+ | watchOS 4.0+ |  |  |  |  |
| Core Motion | Process accelerometer, gyroscope, pedometer, and environment-related events. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 13.0+ | macOS 10.15+ |  | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Core NFC | Detect NFC tags, read messages that contain NDEF data, and save data to writable tags. | iOS 11.0+ | iPadOS 11.0+ | Mac Catalyst 13.1+ |  |  |  |  |  |  |  |  |
| Core Services | Access and manage key operating system services, such as launch and identity services. | iOS 12.0+ | iPadOS 12.0+ | Mac Catalyst 13.0+ | macOS 10.0+ | tvOS 12.0+ | visionOS 1.0+ | watchOS 5.0+ |  |  |  |  |
| Core Spotlight | Add search capabilities to your app, and index your content so people can find it from Spotlight and Safari. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.0+ | macOS 10.13+ |  | visionOS 1.0+ |  |  |  |  |  |
| Core Telephony | Access information about a user’s cellular service provider, such as its unique identifier and whether the carrier allows VoIP. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 14.0+ | macOS 10.10+ |  |  |  |  |  |  |  |
| Core Text | Create text layouts, optimize font handling, and access font metrics and glyph data. | iOS 3.2+ | iPadOS 3.2+ | Mac Catalyst 13.1+ | macOS 10.8+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Core Transferable | Declare a transfer representation for your model types to participate in system sharing and data transfer operations. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| Core Video | Process digital video, including manipulation of individual frames, using a pipeline-based API and support for both Metal and OpenGL. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 13.0+ | macOS 10.4+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 4.0+ |  |  |  |  |
| Core WLAN | Query AirPort interfaces and choose wireless networks. |  |  | Mac Catalyst 13.0+ | macOS 10.6+ |  |  |  |  |  |  |  |
| CoreAudioKit | Add user interfaces to audio units. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.0+ | macOS 10.4+ |  | visionOS 1.0+ |  |  |  |  |  |
| CoreLocationUI | Streamline access to users’ location data through a standard, secure UI. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ |  |  |  | watchOS 10.0+ |  |  |  |  |
| Create ML Components | Create more customizable machine learning models in your app. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 11.0+ |  |  |  |  |
| CryptoTokenKit | Access security tokens and the cryptographic assets they store. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 10.10+ | tvOS 13.0+ | visionOS 1.0+ | watchOS 8.0+ |  |  |  |  |
| Darwin Notify | Send and receive Darwin notifications. | iOS 9.3+ | iPadOS 9.3+ | Mac Catalyst 13.1+ | macOS 10.14+ | tvOS 9.2+ | visionOS 1.0+ | watchOS 2.2+ |  |  |  |  |
| DataDetection | Access and utilize common types of data that the data detection system matches. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ | macOS 12.0+ | tvOS 15.0+ | visionOS 1.0+ | watchOS 8.0+ |  |  |  |  |
| Declared Age Range | Create age-appropriate experiences in your app by asking people to share their age range. | iOS 26.0+ | iPadOS 26.0+ | Mac Catalyst 26.0+ | macOS 26.0+ |  |  |  |  |  |  |  |
| DeveloperToolsSupport | Expose custom views and modifiers in the Xcode library. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ | tvOS 14.0+ | visionOS 1.0+ | watchOS 7.0+ |  |  |  |  |
| DeviceActivity | Monitor device activity with your app extension while maintaining user privacy. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ |  |  |  |  |  |  |  |  |
| DeviceCheck | Reduce fraudulent use of your services by managing device state and asserting app integrity. | iOS 11.0+ | iPadOS 11.0+ | Mac Catalyst 11.0+ | macOS 10.15+ | tvOS 11.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| DeviceDiscoveryExtension | Stream media to a third-party device that a user selects in a system menu. | iOS 16.0+ | iPadOS 16.0+ |  | macOS 15.0+ |  | visionOS 1.0+ |  |  |  |  |  |
| DeviceDiscoveryUI | Display an interface that lets users connect a tvOS app to a mobile device over the local network. |  |  |  |  | tvOS 16.0+ |  |  |  |  |  |  |
| Disk Arbitration | Provides mechanisms to register and block disk mount or unmount events. |  |  | Mac Catalyst 13.0+ | macOS 10.4+ |  |  |  |  |  |  |  |
| Dispatch | Execute code concurrently on multicore hardware by submitting work to dispatch queues managed by the system. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.0+ | macOS 10.10+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Distributed | Build systems that run distributed code across multiple processes and devices. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ |  | watchOS 9.0+ |  |  |  |  |
| dnssd | Discover, publish, and resolve network services on a local area or wide area network. | iOS 10.0+ | iPadOS 10.0+ | Mac Catalyst 13.0+ | macOS 10.12+ | tvOS 10.0+ | visionOS 1.0+ | watchOS 3.0+ |  |  |  |  |
| DockKit | Interact with accessories that track subjects on camera as they move around. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ |  |  |  |  |  |  |  |  |
| Endpoint Security | Develop system extensions that enhance user security. |  |  | Mac Catalyst 13.0+ | macOS 10.15+ |  |  |  |  |  |  |  |
| EnergyKit | Provide a grid forecast for your app to help people choose when to use electricity. | iOS 26.0+ | iPadOS 26.0+ |  |  |  |  |  |  |  |  |  |
| EventKit | Create, view, and edit calendar and reminder events. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 13.1+ | macOS 10.8+ |  | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| EventKit UI | Display an interface for viewing, selecting, and editing calendar events and reminders. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 13.0+ |  |  | visionOS 1.0+ |  |  |  |  |  |
| Exception Handling | Monitor and debug exceptional conditions in code. |  |  | Mac Catalyst 13.0+ | macOS 10.0+ |  |  |  |  |  |  |  |
| Execution Policy | Provide functionality so developer tools can manage execution policy exceptions. |  |  | Mac Catalyst 13.0+ | macOS 10.15+ |  |  |  |  |  |  |  |
| Exposure Notification | Implement a COVID-19 exposure notification system that protects user privacy. | iOS 13.5+ | iPadOS 13.5+ | Mac Catalyst 13.5+ |  |  |  |  |  |  |  |  |
| ExtensionFoundation | Create executable bundles to extend the functionality of other apps. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 17.4+ | visionOS 1.1+ | watchOS 9.0+ |  |  |  |  |
| ExtensionKit | Make custom UI from an app extension available in a host app, and manage the list of enabled and disabled app extensions. | iOS 16.1+ | iPadOS 16.1+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 10.0+ |  |  |  |  |
| External Accessory | Communicate with accessories that connect to a device with the Apple Lightning connector, or with Bluetooth wireless technology. | iOS 3.0+ | iPadOS 3.0+ | Mac Catalyst 13.0+ | macOS 10.13+ | tvOS 10.0+ | visionOS 1.0+ |  |  |  |  |  |
| FamilyControls | Authorize your app to provide parental controls on a device. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ |  |  |  |  |  |  |  |  |
| File Provider | An extension other apps use to access files and folders managed by your app and synced with a remote storage. | iOS 11.0+ | iPadOS 11.0+ | Mac Catalyst 11.0+ | macOS 10.15+ |  | visionOS 1.0+ |  |  |  |  |  |
| File Provider UI | Add actions to the document browser’s context menu. | iOS 11.0+ | iPadOS 11.0+ | Mac Catalyst 15.0+ | macOS 10.15+ |  | visionOS 1.0+ |  |  |  |  |  |
| FinanceKit | Access financial data and interact with Apple Card, Apple Cash, and orders in Wallet. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ |  |  |  |  |  |  |  |  |
| FinanceKitUI | Add orders to Apple Wallet. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ |  |  |  |  |  |  |  |  |
| Finder Sync | Modify the Finder’s user interface to express file synchronization and control. |  |  |  | macOS 10.10+ |  |  |  |  |  |  |  |
| Force Feedback | Control force feedback devices attached to the system. Develop plug-ins that enable communication with force feedback hardware. |  |  | Mac Catalyst 13.0+ | macOS 10.2+ |  |  |  |  |  |  |  |
| Foundation | Access essential data types, collections, and operating-system services to define the base layer of functionality for your app. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.0+ | macOS 10.0+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Foundation Models | Perform tasks with the on-device model that specializes in language understanding, structured output, and tool calling. | iOS 26.0+ | iPadOS 26.0+ | Mac Catalyst 26.0+ | macOS 26.0+ |  | visionOS 26.0+ |  |  |  |  |  |
| FSKit | Implement a file system that runs in user space. |  |  |  | macOS 15.4+ |  |  |  |  |  |  |  |
| Game Controller | Support hardware game controllers in your game. | iOS 7.0+ | iPadOS 7.0+ | Mac Catalyst 13.1+ | macOS 10.9+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| GameKit | Enable players to interact with friends, compare leaderboard ranks, earn achievements, and participate in multiplayer games. | iOS 3.0+ | iPadOS 3.0+ | Mac Catalyst 13.1+ | macOS 10.8+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 3.0+ |  |  |  |  |
| GameplayKit | Architect and organize your game logic. Incorporate common gameplay behaviors such as random number generation, artificial intelligence, pathfinding, and agent behavior. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.0+ | macOS 10.11+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| GameSave | Store and sync your application’s save files in iCloud. | iOS 26.0+ | iPadOS 26.0+ | Mac Catalyst 26.0+ | macOS 26.0+ |  | visionOS 26.0+ |  |  |  |  |  |
| GeoToolbox | Determine place descriptor information for map coordinates. | iOS 26.0+ | iPadOS 26.0+ | Mac Catalyst 26.0+ | macOS 26.0+ | tvOS 26.0+ | visionOS 26.0+ | watchOS 26.0+ |  |  |  |  |
| GLKit | Speed up OpenGL ES or OpenGL app development. Use math libraries, background texture loading, pre-created shader effects, and a standard view and view controller to implement your rendering loop. | iOS 5.0+ | iPadOS 5.0+ |  | macOS 10.8+ | tvOS 9.0+ |  |  |  |  |  |  |
| Group Activities | Create app-specific activities your users can share and experience together. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ | macOS 12.0+ | tvOS 15.0+ | visionOS 1.0+ |  |  |  |  |  |
| GSS | Conduct secure, authenticated network transactions. | iOS 5.0+ | iPadOS 5.0+ | Mac Catalyst 13.0+ | macOS 10.14+ |  | visionOS 1.0+ |  |  |  |  |  |
| HealthKit | Access and share health and fitness data while maintaining the user’s privacy and control. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 17.0+ | macOS 14.0+ |  | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| HomeKit | Configure, control, and communicate with home automation accessories. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 14.0+ |  | tvOS 10.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| hvf | Render Hierarchical Variation Font (HVF) glyph outlines, and support font editors and related tools. | iOS 18.4+ | iPadOS 18.4+ |  | macOS 15.4+ | tvOS 18.4+ | visionOS 2.4+ | watchOS 11.4+ |  |  |  |  |
| Hypervisor | Build virtualization solutions on top of a lightweight hypervisor, without third-party kernel extensions. |  |  |  | macOS 10.10+ |  |  |  |  |  |  |  |
| iAd | The Apple Search Ads iAd Attribution API is a legacy framework for attributing app data that originates from Apple Search Ads campaigns on iOS devices. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 13.0+ |  |  |  |  |  |  |  | After February 7, 2023, all requests made to the Apple Search Ads iAd Attribution API will return with a value of "iad-attribution" = false, or errors. See requestAttributionDetails(_:). Use the AdServices framework for current attribution integration with the doc://com.apple.documentation/documentation/apple_search_ads Campaign Management API for devices using iOS 14.3 and later. Attribution isn’t available for downloads and redownloads from devices using iOS 14.2 or earlier. |
| IdentityDocumentServices | Share mobile documents using the Digital Credentials API. | iOS 26.0+ | iPadOS 26.0+ |  | macOS 26.0+ |  |  |  |  |  |  |  |
| IdentityDocumentServicesUI | Provide an interface so people can present mobile documents. | iOS 26.0+ | iPadOS 26.0+ |  | macOS 26.0+ |  |  |  |  |  |  |  |
| Image I/O | Read and write most image file formats, and access an image’s metadata. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 13.0+ | macOS 10.8+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Image Playground | Present a system interface to generate images based on descriptive information. | iOS 18.1+ | iPadOS 18.1+ | Mac Catalyst 18.1+ | macOS 15.1+ |  | visionOS 2.4+ |  |  |  |  |  |
| ImageCaptureCore | Browse for media devices and control them programmatically from your app. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 10.6+ |  | visionOS 1.0+ |  |  |  |  |  |
| Immersive Media Support | Read and write essential Apple Immersive Video metadata. |  |  |  | macOS 26.0+ |  | visionOS 26.0+ |  |  |  |  |  |
| InputMethodKit | Develop input methods and manage communication with client applications, candidates windows, and input method modes. |  |  |  | macOS 10.5+ |  |  |  |  |  |  |  |
| IOBluetooth | Gain user-space access to Bluetooth devices. |  |  |  | macOS 10.2+ |  |  |  |  |  |  |  |
| IOBluetooth UI | Present an interface through which users can pair their devices with other Bluetooth devices. |  |  |  | macOS 10.2+ |  |  |  |  |  |  |  |
| IOKit | Access hardware devices and drivers from your apps and services. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 13.0+ | macOS 10.0+ |  | visionOS 1.0+ |  |  |  |  | Devices supported on macOS 11 and later require DriverKit. Use IOKit in your apps and services to discover and use devices. |
| IOSurface | Share hardware-accelerated buffer data (framebuffers and textures) across multiple processes. Manage image memory more efficiently. | iOS 11.0+ | iPadOS 11.0+ | Mac Catalyst 13.0+ | macOS 10.6+ | tvOS 11.0+ | visionOS 1.0+ |  |  |  |  |  |
| IOUSBHost | Create host-mode user space drivers for USB devices. |  |  | Mac Catalyst 14.0+ | macOS 10.15+ |  |  |  |  |  |  |  |
| iTunes Library | Retrieve the properties of the media in the user’s iTunes library. |  |  | Mac Catalyst 14.0+ | macOS 10.13+ |  |  |  |  |  |  |  |
| JavaScriptCore | Evaluate JavaScript programs from within an app, and support JavaScript scripting of your app. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 13.0+ | macOS 10.5+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| Journaling Suggestions | Display a set of recent, personal events that inspire someone to contribute to your app’s creative workflow. | iOS 17.2+ | iPadOS 26.0+ |  |  |  |  |  |  |  |  |  |
| Kernel | Develop kernel-resident device drivers and kernel extensions. |  |  |  | macOS 10.0+ |  |  |  |  |  |  |  |
| Latent Semantic Mapping | Classify text and other token-based content into developer-defined categories. |  |  | Mac Catalyst 13.1+ | macOS 10.5+ |  |  |  |  |  |  |  |
| LightweightCodeRequirements | Test the identity of executable code on disk and in running processes. | iOS 17.4+ | iPadOS 17.4+ | Mac Catalyst 17.4+ | macOS 14.4+ |  |  |  |  |  |  |  |
| Link Presentation | Fetch, provide, and present rich links in your app. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 10.15+ | tvOS 14.0+ | visionOS 1.0+ |  |  |  |  |  |
| LiveCommunicationKit | Initiate and handle VoIP and cellular conversations, coordinate them with other communication apps and the system, and get ready to be a default calling or dialer app. | iOS 17.4+ | iPadOS 17.4+ | Mac Catalyst 17.4+ |  |  | visionOS 1.1+ | watchOS 10.4+ |  |  |  |  |
| Local Authentication | Authenticate users biometrically or with a passphrase they already know. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.0+ | macOS 10.10+ |  | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| Local Authentication Embedded UI | Present a standard local authentication view icon in a custom authentication view. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 12.0+ |  | visionOS 1.0+ |  |  |  |  |  |
| LockedCameraCapture | Capture content with your app’s camera experience when the device is locked. | iOS 18.0+ | iPadOS 18.0+ | Mac Catalyst 18.0+ |  |  |  |  |  |  |  |  |
| MailKit | Secure, customize, and act on email messages that users send and receive. |  |  |  | macOS 12.0+ |  |  |  |  |  |  |  |
| ManagedApp | Customize your app for managed deployments by providing configurable features that rely on secure access to secrets and data that an administrator provisions. | iOS 18.4+ | iPadOS 18.4+ |  |  |  | visionOS 2.4+ |  |  |  |  |  |
| ManagedAppDistribution | Manage the distribution of apps within an organization. | iOS 17.2+ | iPadOS 17.2+ |  |  |  |  |  |  |  |  |  |
| ManagedSettings | Access and change settings with your app while maintaining user privacy and control. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ |  |  |  |  |  |  |  |  |
| ManagedSettingsUI | Define and configure the appearance of shielding views. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ |  |  |  |  |  |  |  |  |
| MapKit | Display map or satellite imagery within your app, call out points of interest, and determine placemark information for map coordinates. | iOS 3.0+ | iPadOS 3.0+ | Mac Catalyst 13.0+ | macOS 10.9+ | tvOS 9.2+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| MarketplaceKit | Create an alternative app marketplace, distribute your app on an alternative app marketplace, or distribute your app from your website. | iOS 17.4+ | iPadOS 18.0+ |  |  |  |  |  |  |  |  |  |
| Matter | Communicate with and control smart home devices from a variety of manufacturers. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.1+ | macOS 13.0+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| MatterSupport | Coordinate and control compatible smart home accessories. | iOS 16.1+ | iPadOS 16.1+ | Mac Catalyst 14.0+ | macOS 14.0+ |  | visionOS 1.0+ |  |  |  |  |  |
| Media Accessibility | Make your app’s media more accessible by supporting people’s systemwide preferences for video and audio content. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 13.0+ | macOS 10.9+ | tvOS 17.0+ | visionOS 1.0+ |  |  |  |  |  |
| Media Player | Find and play songs, audio podcasts, audio books, and more from within your app. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.1+ | macOS 10.12.1+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 5.0+ |  |  |  |  |
| Media Setup | Enable users to configure HomePod speakers to stream music directly from your media service. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 15.4+ |  |  | visionOS 1.0+ |  |  |  |  |  |
| Media Toolbox | Enable support for media format readers; tap and process audio from an audio mix. | iOS 6.0+ | iPadOS 6.0+ | Mac Catalyst 6.0+ | macOS 10.9+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| MediaExtension | This framework provides a means for developers to create format readers, video decoders, and RAW processors for media that the system doesn’t natively support. |  |  | Mac Catalyst 18.0+ | macOS 15.0+ |  |  |  |  |  |  |  |
| Message UI | Create a user interface for composing email and text messages, so users can edit and send messages without leaving your app. | iOS 3.0+ | iPadOS 3.0+ | Mac Catalyst 13.0+ |  |  | visionOS 1.0+ |  |  |  |  |  |
| Messages | Create app extensions that allow users to send text, stickers, media files, and interactive messages. | iOS 10.0+ | iPadOS 10.0+ | Mac Catalyst 14.0+ |  |  |  |  |  |  |  |  |
| Metal | Render advanced 3D graphics and compute data in parallel with graphics processors. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.0+ | macOS 10.11+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| Metal Performance Shaders | Optimize graphics and compute performance with kernels that are fine-tuned for the unique characteristics of each Metal GPU family. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.0+ | macOS 10.13+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| Metal Performance Shaders Graph | Build, compile, and execute compute graphs utilizing all the different compute devices on the platform, including GPU, CPU, and Neural Engine. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ | tvOS 14.0+ | visionOS 1.0+ |  |  |  |  |  |
| MetalFX | Boost your Metal app’s performance by upscaling lower-resolution content to save GPU time. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ |  | visionOS 1.0+ |  |  |  |  |  |
| MetalKit | Build Metal apps quicker and easier using a common set of utility classes. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.0+ | macOS 10.11+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| MetricKit | Aggregate and analyze per-device reports on exception and crash diagnostics and on power and performance metrics. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 12.0+ |  | visionOS 1.0+ |  |  |  |  |  |
| Model I/O | Import, export, and manipulate 3D models using a common infrastructure that integrates MetalKit, GLKit, and SceneKit. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.0+ | macOS 10.11+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| Multipeer Connectivity | Support peer-to-peer connectivity and the discovery of nearby devices. | iOS 7.0+ | iPadOS 7.0+ | Mac Catalyst 13.0+ | macOS 10.10+ | tvOS 10.0+ | visionOS 1.0+ |  |  |  |  |  |
| MusicKit | Integrate your app with Apple Music. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ | macOS 12.0+ | tvOS 15.0+ | visionOS 1.0+ | watchOS 8.0+ |  |  |  |  |
| Natural Language | Analyze natural language text and deduce its language-specific metadata. | iOS 12.0+ | iPadOS 12.0+ | Mac Catalyst 13.0+ | macOS 10.14+ | tvOS 12.0+ | visionOS 1.0+ | watchOS 5.0+ |  |  |  |  |
| Nearby Interaction | Locate and interact with nearby devices using identifiers, distance, and direction. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ |  |  | watchOS 8.0+ |  |  |  |  |
| Network | Create network connections to send and receive data using transport and security protocols. | iOS 12.0+ | iPadOS 12.0+ | Mac Catalyst 13.0+ | macOS 10.14+ | tvOS 12.0+ | visionOS 1.0+ | watchOS 6.0+ |  |  |  |  |
| Network Extension | Customize and extend core networking features. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.1+ | macOS 10.10+ | tvOS 17.0+ | visionOS 1.0+ | watchOS 7.0+ |  |  |  |  |
| Objective-C Runtime | Gain low-level access to the Objective-C runtime and the Objective-C root types. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.0+ | macOS 10.0+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Observation | Make responsive apps that update the presentation when underlying data changes. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ | macOS 14.0+ | tvOS 17.0+ | visionOS 1.0+ | watchOS 10.0+ |  |  |  |  |
| Open Directory | Authenticate users, and search for contact information in Open Directory and LDAP directories. |  |  | Mac Catalyst 13.0+ | macOS 10.6+ |  |  |  |  |  |  |  |
| os | Coordinate the scheduling and synchronization of your app’s tasks, and log information to the console to diagnose issues. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.1+ | macOS 10.10+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| OSLog | A unified logging system for the reading of historical data. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ | macOS 10.15+ | tvOS 15.0+ | visionOS 1.0+ | watchOS 8.0+ |  |  |  |  |
| PaperKit | Add drawings, shapes, and a consistent markup experience to your app. | iOS 26.0+ | iPadOS 26.0+ |  | macOS 26.0+ |  | visionOS 26.0+ |  |  |  |  |  |
| Paravirtualized Graphics | Add graphics acceleration to your guest driver stack. |  |  | Mac Catalyst 14.0+ | macOS 11.0+ |  |  |  |  |  |  |  |
| PassKit (Apple Pay and Wallet) | Process Apple Pay payments in your app, and create and distribute passes for the Wallet app. | iOS 6.0+ | iPadOS 6.0+ | Mac Catalyst 13.0+ | macOS 11.0+ |  | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| PDFKit | Display and manipulate PDF documents in your apps. | iOS 11.0+ | iPadOS 11.0+ | Mac Catalyst 11.0+ | macOS 10.4+ |  | visionOS 1.0+ |  |  |  |  |  |
| PencilKit | Capture touch and Apple Pencil input as a drawing, and display that content from your app. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 10.15+ |  | visionOS 1.0+ |  |  |  |  |  |
| PermissionKit | Create communication experiences between a child and their parent or guardian. | iOS 26.0+ | iPadOS 26.0+ | Mac Catalyst 26.0+ | macOS 26.0+ |  | visionOS 26.0+ |  |  |  |  |  |
| PHASE | Create dynamic audio experiences in your game or app that react to events and cues in the environment. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ | macOS 12.0+ | tvOS 15.0+ | visionOS 1.0+ |  |  |  |  |  |
| PhotoKit | Work with image and video assets that the Photos app manages, including those from iCloud Photos and Live Photos. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.1+ | macOS 10.11+ | tvOS 10.0+ | visionOS 1.0+ | watchOS 10.0+ |  |  |  |  |
| Playground Bluetooth | Display and manage connections to Bluetooth peripherals in Swift Playgrounds. |  |  |  |  |  |  |  | Swift Playgrounds 2.0+ |  |  |  |
| Playground Support | Share playground data, manage live views, and control the execution of a playground. |  |  |  | macOS 12.0+ |  |  |  | Swift Playgrounds 2.0+ |  |  |  |
| Preference Panes | Integrate your app’s custom preferences into the System Preferences app. |  |  | Mac Catalyst 14.0+ | macOS 10.1+ |  |  |  |  |  |  |  |
| ProximityReader | Read contactless physical and digital wallet cards using your iPhone. | iOS 15.4+ | iPadOS 15.4+ | Mac Catalyst 15.4+ |  |  |  |  |  |  |  |  |
| Push to Talk | Display the system user interface for your app’s Push to Talk services. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ |  |  |  |  |  |  |  |  |
| PushKit | Respond to push notifications related to your app’s complications, file providers, and VoIP services. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.0+ | macOS 10.15+ |  | visionOS 1.0+ | watchOS 6.0+ |  |  |  |  |
| Quartz | Allow users to browse, edit, and save images, using slideshows and Core Image filters. |  |  |  | macOS 10.4+ |  |  |  |  |  |  |  |
| Quick Look | Create previews of files to use inside your app, or perform simple edits on previews. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 13.0+ | macOS 10.5+ |  | visionOS 1.0+ |  |  |  |  |  |
| Quick Look Thumbnailing | Generate thumbnails for common file types and add a Thumbnail Extension to your app to enable others to create thumbnails of your custom files. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 10.15+ |  | visionOS 1.0+ |  |  |  |  |  |
| Quick Look UI | Create previews of files to use inside your macOS app. |  |  |  | macOS 12.0+ |  |  |  |  |  |  |  |
| RealityKit | Simulate and render 3D content for use in your augmented reality apps. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.1+ | macOS 10.15+ | tvOS 26.0+ | visionOS 1.0+ |  |  |  |  |  |
| RegexBuilder | Use an expressive domain-specific language to build regular expressions, for operations like searching and replacing in text. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ |  | watchOS 9.0+ |  |  |  |  |
| RelevanceKit | Provide on-device intelligence with contextual clues that increase your widget’s visibility on Apple Watch. | iOS 26.0+ | iPadOS 26.0+ | Mac Catalyst 26.0+ | macOS 26.0+ |  | visionOS 26.0+ | watchOS 26.0+ |  |  |  |  |
| ReplayKit | Record or stream video from the screen, and audio from the app and microphone. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.0+ | macOS 11.0+ | tvOS 10.0+ | visionOS 1.0+ |  |  |  |  |  |
| RoomPlan | Create a 3D model of a room by interactively guiding people to scan their physical environment using a device’s camera. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ |  |  |  |  |  |  |  |  |
| Safari Services | Enable web views and services in your app. | iOS 7.0+ | iPadOS 7.0+ | Mac Catalyst 13.0+ | macOS 10.12+ |  | visionOS 1.0+ |  |  |  |  |  |
| SafetyKit | Detect and respond to car crash events in your app. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.1+ | macOS 13.0+ |  |  | watchOS 10.1+ |  |  |  |  |
| Screen Saver | Animate screen savers, and interact with the screen saver infrastructure. |  |  |  | macOS 10.0+ |  |  |  |  |  |  |  |
| Screen Time | Share and manage web-usage data, and observe changes made by a parent or guardian. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ |  |  |  |  |  |  |  |
| ScreenCaptureKit | Filter and select screen content and stream it to your app. |  |  | Mac Catalyst 18.2+ | macOS 12.3+ |  |  |  |  |  |  |  |
| Scripting Bridge | Automate scriptable apps by sending and receiving Apple events. |  |  | Mac Catalyst 13.0+ | macOS 10.5+ |  |  |  |  |  |  |  |
| Security | Secure the data your app manages, and control access to your app. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.0+ | macOS 10.0+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Security Foundation | Restrict a user’s access to particular features in your Mac app or daemon. |  |  | Mac Catalyst 13.0+ | macOS 10.3+ |  |  |  |  |  |  |  |
| Security Interface | Provide user interface elements for security features such as authorization, access to digital certificates, and access to items in keychains. |  |  |  | macOS 10.3+ |  |  |  |  |  |  |  |
| SensitiveContentAnalysis | Provide a safer experience in your app by detecting and alerting users to nudity in images and videos before displaying them onscreen. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ | macOS 14.0+ |  |  |  |  |  |  |  |
| SensorKit | Retrieve data and derived metrics from sensors on an iPhone, or paired Apple Watch. | iOS 14.0+ | iPadOS 14.0+ |  |  |  |  |  |  |  |  |  |
| Service Management | Manage startup items, launch agents, and launch daemons from within an app. |  |  | Mac Catalyst 13.0+ | macOS 10.6+ |  |  |  |  |  |  |  |
| ServicesAccountLinking | Link reseller accounts with Apple Media & Purchases accounts. | iOS 16.4+ | iPadOS 16.4+ | Mac Catalyst 16.4+ |  |  |  |  |  |  |  |  |
| ShaderGraph | Create custom materials and effects for 3D content in Reality Composer Pro. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ | macOS 15.0+ | tvOS 26.0+ | visionOS 1.0+ |  |  |  |  |  |
| Shared with You | Surface shared content and collaborate in your app. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ | visionOS 1.0+ |  |  |  |  |  |
| ShazamKit | Find information about a specific audio recording when a segment of it’s part of captured sound in the Shazam catalog or your custom catalog. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ | macOS 12.0+ | tvOS 15.0+ | visionOS 1.0+ | watchOS 8.0+ |  |  |  |  |
| SiriKit | Empower users to interact with their devices through voice, intelligent suggestions, and personalized workflows. | iOS 10.0+ | iPadOS 10.0+ | Mac Catalyst 13.0+ | macOS 12.0+ | tvOS 14.0+ | visionOS 1.0+ | watchOS 3.2+ |  |  |  |  |
| SMS and Call Reporting | Create app extensions to manage and report unwanted SMS messages and spam calls. | iOS 11.0+ | iPadOS 11.0+ | Mac Catalyst 13.1+ | macOS 10.15+ |  | visionOS 1.0+ |  |  |  |  |  |
| Social | Post content to supported social networking services, using standard system interfaces. | iOS 6.0+ | iPadOS 6.0+ | Mac Catalyst 13.0+ | macOS 10.8+ |  |  |  |  |  |  |  |
| Sound Analysis | Classify various sounds by analyzing audio files or streams. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.1+ | macOS 10.15+ | tvOS 13.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| Spatial | Create and manipulate 3D mathematical primitives. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| Speech | Perform speech recognition on live or prerecorded audio, and receive transcriptions, alternative interpretations, and confidence levels of the results. | iOS 10.0+ | iPadOS 10.0+ | Mac Catalyst 13.1+ | macOS 10.15+ |  | visionOS 1.0+ |  |  |  |  |  |
| SpriteKit | Add high-performance 2D content with smooth animations to your app, or create a game with a high-level set of 2D game-based tools. | iOS 7.0+ | iPadOS 7.0+ | Mac Catalyst 13.0+ | macOS 10.9+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 10.0+ |  |  |  |  |
| StoreKit | Support In-App Purchases and interactions with the App Store. | iOS 3.0+ | iPadOS 3.0+ | Mac Catalyst 13.0+ | macOS 10.7+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 6.2+ |  |  |  |  |
| StoreKit Test | Create and automate tests in Xcode for your app’s subscription and in-app purchase transactions, and SKAdNetwork implementations. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ | tvOS 14.0+ | visionOS 1.0+ | watchOS 7.4+ |  |  |  |  |
| Swift | Build apps using a powerful open language. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 13.0+ | macOS 10.10+ | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Swift Charts | Construct and customize charts on every Apple platform. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| Swift Testing | Create and run tests for your Swift packages and Xcode projects. |  |  |  |  |  |  |  |  | Swift 6.0+ | Xcode 16.0+ |  |
| SwiftData | Write your model code declaratively to add managed persistence and efficient model fetching. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ | macOS 14.0+ | tvOS 17.0+ | visionOS 1.0+ | watchOS 10.0+ |  |  |  |  |
| SwiftUI | Declare the user interface and behavior for your app on every platform. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 10.15+ | tvOS 13.0+ | visionOS 1.0+ | watchOS 6.0+ |  |  |  |  |
| Symbols | Apply universal animations to symbol-based images. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ | macOS 14.0+ | tvOS 17.0+ | visionOS 1.0+ | watchOS 10.0+ |  |  |  |  |
| Synchronization | Build synchronization constructs using low-level, primitive operations. | iOS 18.0+ | iPadOS 18.0+ | Mac Catalyst 18.0+ | macOS 15.0+ | tvOS 18.0+ | visionOS 2.0+ | watchOS 11.0+ |  |  |  |  |
| System | Perform low-level file operations using type-safe APIs. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ | tvOS 14.0+ | visionOS 1.0+ | watchOS 7.0+ |  |  |  |  |
| System Configuration | Allow applications to access a device’s network configuration settings. Determine the reachability of the device, such as whether Wi-Fi or cell connectivity are active. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.1+ | macOS 10.1+ | tvOS 9.0+ | visionOS 1.0+ |  |  |  |  |  |
| System Extensions | Install and manage user space code that extends the capabilities of macOS. |  |  |  | macOS 10.15+ |  |  |  |  |  |  |  |
| TabletopKit | Create multiplayer spatial games on a virtual table surface and use FaceTime to invite players. |  |  |  |  |  | visionOS 2.0+ |  |  |  |  |  |
| TabularData | Import, organize, and prepare a table of data to train a machine learning model. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 15.0+ | macOS 12.0+ | tvOS 15.0+ | visionOS 1.0+ | watchOS 8.0+ |  |  |  |  |
| TelephonyMessagingKit | Send and receive standards-based messages over cellular networks. | iOS 26.0+ | iPadOS 26.0+ |  |  |  |  |  |  |  |  |  |
| ThreadNetwork | Create robust, smart device networks using Thread Border Routers. | iOS 15.0+ | iPadOS 15.0+ | Mac Catalyst 16.1+ | macOS 14.0+ |  | visionOS 1.0+ |  |  |  |  |  |
| TipKit | Display tips that help people discover features in your app. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ | macOS 14.0+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 10.0+ |  |  |  |  |
| Touch Controller | Integrate onscreen touch controls into your Metal-based games. | iOS 26.0+ | iPadOS 26.0+ | Mac Catalyst 26.0+ |  |  | visionOS 26.0+ |  |  |  |  |  |
| Translation | Translate text in your app from one language to another. | iOS 17.4+ | iPadOS 17.4+ |  | macOS 14.4+ |  |  |  |  |  |  |  |
| TranslationUIProvider | Provide UI for translations of text people select. | iOS 18.4+ | iPadOS 18.4+ |  |  |  |  |  |  |  |  |  |
| TV Services | Display content and descriptions, provide channel guides, and support multiple users on Apple TV. |  |  |  |  | tvOS 9.0+ |  |  |  |  |  |  |
| TVUIKit | Show common user interface elements from Apple TV in your native app. |  |  |  |  | tvOS 12.0+ |  |  |  |  |  |  |
| UIKit | Construct and manage a graphical, event-driven user interface for your iOS, iPadOS, or tvOS app. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.0+ |  | tvOS 9.0+ | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| Uniform Type Identifiers | Provide uniform type identifiers that describe file types for storage or transfer. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ | tvOS 14.0+ | visionOS 1.0+ | watchOS 7.0+ |  |  |  |  |
| User Notifications | Push user-facing notifications to the user’s device from a server, or generate them locally from your app. | iOS 10.0+ | iPadOS 10.0+ | Mac Catalyst 13.0+ | macOS 10.14+ | tvOS 10.0+ | visionOS 1.0+ | watchOS 3.0+ |  |  |  |  |
| User Notifications UI | Customize the interface that displays local and remote notifications. | iOS 10.0+ | iPadOS 10.0+ | Mac Catalyst 14.0+ | macOS 11.0+ |  | visionOS 1.0+ |  |  |  |  |  |
| Video Subscriber Account | Support TV provider and Apple TV app functionality. | iOS 10.0+ | iPadOS 10.0+ |  | macOS 10.14+ | tvOS 10.0+ | visionOS 1.0+ |  |  |  |  |  |
| Video Toolbox | Work directly with hardware-accelerated video encoding and decoding capabilities. | iOS 6.0+ | iPadOS 6.0+ | Mac Catalyst 13.0+ | macOS 10.8+ | tvOS 10.2+ | visionOS 1.0+ |  |  |  |  |  |
| Virtualization | Create virtual machines and run macOS and Linux-based operating systems. |  |  |  | macOS 11.0+ |  |  |  |  |  |  |  |
| VisionKit | Identify and extract information in the environment using the device’s camera, or in images that your app displays. | iOS 13.0+ | iPadOS 13.0+ | Mac Catalyst 13.0+ | macOS 13.0+ |  | visionOS 1.0+ |  |  |  |  |  |
| Visual Intelligence | Include your app’s content in search results that visual intelligence provides. | iOS 26.0+ | iPadOS 26.0+ | Mac Catalyst 26.0+ |  |  |  |  |  |  |  |  |
| vmnet | Connect with network interfaces to read and write packets on guest operating systems. |  |  | Mac Catalyst 13.0+ | macOS 10.10+ |  |  |  |  |  |  |  |
| Wallet Orders | Create, distribute, and update orders in Wallet. | iOS 16.0+ | iPadOS 16.0+ |  | macOS 13.0+ |  |  |  |  |  |  |  |
| Wallet Passes | Create, distribute, and update passes for the Wallet app. | iOS 6.0+ | iPadOS 6.0+ |  |  |  |  | watchOS 2.0+ |  |  |  |  |
| Watch Connectivity | Implement two-way communication between an iOS app and its paired watchOS app. | iOS 9.0+ | iPadOS 9.0+ | Mac Catalyst 13.0+ |  |  | visionOS 1.0+ | watchOS 2.0+ |  |  |  |  |
| WatchKit | Build watchOS apps that use features the app delegate monitors or controls, such as background tasks and extended runtime sessions. |  |  |  |  |  |  | watchOS 2.0+ |  |  |  |  |
| WeatherKit | Deliver weather conditions and alerts to your users. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 16.0+ | macOS 13.0+ | tvOS 16.0+ | visionOS 1.0+ | watchOS 9.0+ |  |  |  |  |
| WebKit | Integrate web content seamlessly into your app, and customize content interactions to meet your app’s needs. | iOS 16.0+ | iPadOS 16.0+ | Mac Catalyst 13.1+ | macOS 10.2+ |  | visionOS 1.0+ |  |  |  |  |  |
| Wi-Fi Aware | Securely pair and connect to external devices over peer-to-peer Wi-Fi. | iOS 26.0+ | iPadOS 26.0+ |  |  |  |  |  |  |  |  |  |
| Wi-Fi Infrastructure-BETA | Share Wi-Fi network credentials securely between devices and connected accessories. | iOS 26.2+Beta | iPadOS 26.2+Beta |  |  |  |  |  |  |  |  |  |
| WidgetKit | Extend the reach of your app by creating widgets, watch complications, Live Activities, and controls. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ |  | visionOS 26.0+ | watchOS 9.0+ |  |  |  |  |
| WirelessInsights | Receive notifications for anticipated changes in cellular data service conditions. | iOS 26.0+ | iPadOS 26.0+ |  |  |  |  |  |  |  |  |  |
| WorkoutKit | Create, preview, and sync workout compositions to the Workout app. | iOS 17.0+ | iPadOS 17.0+ | Mac Catalyst 17.0+ |  |  |  | watchOS 10.0+ |  |  |  |  |
| XcodeKit | Create extensions to add commands to the Xcode source editor. |  |  |  | macOS 10.12+ |  |  |  |  |  |  |  |
| xcselect | Access the path of the macOS SDK available on the host system. |  |  | Mac Catalyst 13.0+ | macOS 10.15+ |  |  |  |  |  |  |  |
| XCTest | Create and run unit tests, performance tests, and UI tests for your Xcode project. |  |  |  |  |  |  |  |  |  | xcode 5.0+ |  |
| XCUIAutomation | Replicate sequences of interactions and make sure that your app’s user interface behaves as intended. |  |  |  |  |  |  |  |  |  | Xcode 16.3+ |  |
| XPC | Access a low-level interprocess communication mechanism. | iOS 17.4+ | iPadOS 17.4+ | Mac Catalyst 13.0+ | macOS 10.10+ |  |  |  |  |  |  |  |


# Deprecated Frameworks

| Framework | <div style="width:290px">Description</div> | iOS | iPadOS | Mac Catalyst | macOS | tvOS | visionOS | watchOS | <div style="width:290px">NOTE</div> |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Accounts | Help users access and manage their external accounts from within your app, without requiring them to enter login credentials. | iOS 5.0+ | iPadOS 5.0+ | Mac Catalyst 13.0+ | macOS 10.8+ |  |  |  | The Accounts framework is deprecated. For new apps, instead of using Accounts, contact the provider of the service you integrate with, to get access to their SDK or documentation about managing accounts with their service. |
| Assets Library | Access the assets in a user’s media library. | iOS 4.0+ | iPadOS 4.0+ | Mac Catalyst 14.0+ |  |  |  |  | The Assets Library framework is deprecated as of iOS 9.0. Instead, use the PhotoKit framework, which in iOS 8.0 and later provides more features and better performance for working with a user’s photo library. |
| Audio Unit | Add sophisticated audio manipulation and processing capabilities to your app. | iOS 2.0+ | iPadOS 2.0+ | Mac Catalyst 13.0+ | macOS 10.0+ | tvOS 9.0+ | visionOS 1.0+ |  | Use the Audio Unit types in Audio Toolbox instead. |
| Media Library | Access read-only collections of the user’s multimedia content. |  |  | Mac Catalyst 13.0+ | macOS 10.9+ |  |  |  | Use the PhotoKit and iTunes Library frameworks instead. |
| ML Compute | Accelerate training and validation of neural networks across the CPU and one or more GPUs. | iOS 14.0+ | iPadOS 14.0+ | Mac Catalyst 14.0+ | macOS 11.0+ | tvOS 14.0+ |  |  | ML Compute is deprecated. Instead, use BNNS for CPU tasks, Metal Performance Shaders for GPU work, and Core ML for tensor APIs. |
| Notification Center | Create and manage widgets for the Today view. | iOS 8.0+ | iPadOS 8.0+ | Mac Catalyst 8.0+ | macOS 10.10+ |  |  |  | Use WidgetKit instead. |
| SceneKit | Create 3D games and add 3D content to apps using high-level scene descriptions, and easily add animations, physics simulation, particle effects, and realistic physically based rendering. | iOS 8.0–26.0 | iPadOS 8.0–26.0 | Mac Catalyst 13.1–26.0 | macOS 10.8–26.0 | tvOS 9.0–26.0 | visionOS 1.0–26.0 | watchOS 3.0–26.0 | SceneKit is deprecated, use RealityKit instead. For more information, see WWDC25 session 288: Bring your SceneKit projects to RealityKit. |
| OpenGL ES | Create 3D and 2D graphics effects with this compact, efficient subset of OpenGL. | iOS 2.0–12.0 | iPadOS 2.0–12.0 |  |  | tvOS 9.0–12.0 | visionOS 1.0–1.0 |  |  |
| TVMLKit | Create client-server apps by incorporating JavaScript and TVML files in your binary app. |  |  |  |  | tvOS 9.0+ |  |  | TVMLKit is deprecated in tvOS 18 and later. Instead, develop apps for tvOS with SwiftUI or UIKit. For more information, see Creating a tvOS media catalog app in SwiftUI. |
| TVMLKit JS | Create tvOS client-server apps using web technologies to stream media and respond to events. |  |  |  |  | tvOS 10.0+ |  |  | TVMLKit JS is deprecated in tvOS 18 and later. Instead, develop apps for tvOS with SwiftUI or UIKit. For more information, see Creating a tvOS media catalog app in SwiftUI. |

# Services

| Service | <div style="width:290px">Description</div> | API | OS | <div style="width:290px">NOTE</div> |
| --- | --- | --- | --- | --- |
| Account & Organizational Data Sharing | Provide people with the ability to authorize your apps and websites that access information about them on Apple REST services, like Roster API. | AccountOrganizationalDataSharing 1.0+ |  |  |
| Account Data Transfer | Download App Store information and app-install activity on behalf of your app’s users. | Account Data Transfer 1.0+ |  |  |
| Advanced Commerce API | Support In-App Purchases through the App Store for exceptionally large catalogs of custom one-time purchases, subscriptions, and subscriptions with optional add-ons. | Advanced Commerce API 1.0+ |  |  |
| App Data Transfer | Download App Store information and app-install activity about your app. | App Data Transfer 1.0+ |  |  |
| App Store Connect API | Automate the tasks you perform on the Apple Developer website and in App Store Connect. | App Store Connect API 1.0+ |  |  |
| App Store Server Notifications | Monitor In-App Purchase events in real time and learn of unreported external purchase tokens, with server notifications from the App Store. | App Store Server Notifications 1.0+ |  | The App Store Server Notifications V1 endpoint and version 1 notifications, notification_type, are deprecated. Implement the App Store Server Notifications V2 endpoint on your server to receive version 2 notifications instead. |
| Apple Ads | Drive app discovery by creating and managing campaigns with the Apple Ads Campaign Management API. | Apple Ads 2.0+ |  |  |
| Apple Maps Server API | Reduce API calls and conserve device power by streamlining your app’s georelated searches. | Apple Maps Server API 1.2+ |  |  |
| Apple Music API | Integrate streaming music with catalog and personal content. | Apple Music 1.0+ |  |  |
| Apple Music Feed | Access the content of the Apple Music Catalog in bulk. | AppleMusicFeed 1.0+ |  |  |
| Apple News | Design, create, and publish signature content for Apple News. | Apple News API 1.0+, Apple News Format 1.7+ |  |  |
| Apple Pay Merchant Token Management API | Retrieve and manage payment life-cycle events for your Apple Pay merchant tokens. | App Store Connect API 1.0+ |  |  |
| Apple Pay Web Merchant Registration API | Manage merchant registration through your web platform. | Apple Pay Web Merchant Registration API 1.0+ |  |  |
| Automatic Sign-In API | Manage sign-in tokens from your web server that facilitate single sign-on across the devices of your media-streaming service customers. | Automatic Sign-In API 1.0+ |  |  |
| ClassKit Catalog API | Declare the activities supported by your educational app through a web interface. | ClassKit 1.0+ |  |  |
| Device Management | Manage your organization’s devices remotely. | Device Assignment Services 5.0+, VPP License Management 1.0+ | iOS 13.0+, iPadOS 13.0+, macOS 10.15+, tvOS 13.0+, visionOS 1.1+, watchOS 6.0+ |  |
| External Purchase Server API | Send and manage reports you send to Apple for tokens you receive when your app provides external purchases for digital goods and services. | External Purchase Server API 1.0.0+ |  |  |
| iWork Document Exporting API | Convert iWork documents to Portable Document Format (PDF) files using a web API. | iWork 14.0+ |  |  |
| Maps Web Snapshots | Create a static image of a map from a URL. | Maps Web Snapshots 1.0+ |  |  |
| Notary API | Submit your macOS software for notarization through a web interface. | Notary API 2.0.0+ |  |  |
| Retention Messaging API | Provide a reason for customers to stay subscribed with a preconfigured message that you can choose in real time, appropriate to the product and locale. | Retention Messaging API 1.0+ |  |  |
| Roster API | Read information about people and classes from an Apple School Manager organization. | Roster API 1.0.0+ |  |  |
| Sign in with Apple | Provide users the ability to sign in to your apps and websites using their Apple Account. | Sign in with Apple JS 1.0+, Sign in with Apple REST API 1.0+ |  |  |
| Siri Event Suggestions Markup | Update users’ calendars and inform suggestions from Siri with reservation data embedded in email and webpages. | Siri Event Suggestions Markup 1.0+ |  |  |
| SiriKit Cloud Media | Stream music directly to HomePod speakers from your media service. | SiriKit Cloud Media 1.0.2+ |  |  |
| SKAdNetwork for Web Ads | Attribute app-install campaigns that originate on the web. | SKAdNetwork for Web Ads 1.0+ |  |  |
| WeatherKit REST API | Obtain historical, current, and predictive weather for your app or service. | Weather API 1.0.0+ |  | Using this API requires attribution. See WeatherKit - Data Sources to learn more. |

# Deprecated Services

| Service | <div style="width:290px">Description</div> | API | <div style="width:290px">NOTE</div> |
| --- | --- | --- | --- |
| App Store Receipts | Validate app and In-App Purchase receipts with the App Store. | App Store Receipts 1.0–1.7 | Receipts are deprecated. To validate In-App Purchases on your server without using receipts, call the App Store Server API to get Apple-signed transaction and subscription information for your customers, or verify the AppTransaction and Transaction signed data that your app obtains. You can also get the same signed transaction and subscription information from the App Store Server Notifications V2 endpoint. |

# Tools

| Title | <div style="width:290px">Description</div> | URL |
| --- | --- | --- |
| DocC | Produce rich API reference documentation and interactive tutorials for your Swift framework or package. | https://www.swift.org/documentation/docc/ |
| ResearchKit | ResearchKit is an open source software framework that makes it easy to create apps for medical research or for other research projects. | https://github.com/ResearchKit |
| Installer JS | Manage and customize the installation and distribution experience. | https://developer.apple.com/documentation/installer_js |
| PackageDescription | Create reusable code, organize it in a lightweight way, and share it across your projects and with other developers. | https://developer.apple.com/documentation/PackageDescription |
| Reality Composer Pro | Build, create, and design 3D content for your RealityKit apps. | https://developer.apple.com/documentation/RealityComposerPro |
| Safari Developer Features | Inspect, debug, and test web content in Safari, in other apps, and on other devices including iPhone and iPad. | https://developer.apple.com/documentation/safari-developer-tools |
| Sample Code Library | Enhance and expand your knowledge of Apple technologies by exploring the full library of sample code projects. | https://developer.apple.com/documentation/SampleCode |
| Swift packages | Create reusable code, organize it in a lightweight way, and share it across Xcode projects and with other developers. | https://developer.apple.com/documentation/Xcode/swift-packages |
| Swift Playgrounds | Learn to write apps, repurpose sample code, create, and share learning experiences in Swift Playgrounds. | https://developer.apple.com/documentation/swift-playgrounds |
| Technology Overviews | Learn about the wide range of technologies you use to develop software for Apple platforms. | https://developer.apple.com/documentation/TechnologyOverviews |
| Xcode | Build, test, and submit your app with Apple’s integrated development environment. | https://developer.apple.com/documentation/Xcode |
| Xcode Cloud | Automatically build, test, and distribute your apps with Xcode Cloud to verify changes and create high-quality apps. | https://developer.apple.com/documentation/Xcode/Xcode-Cloud |

# DriverKit

| Framework | <div style="width:290px">Description</div> | DriverKit | macOS | iOS | iPadOS |
| --- | --- | --- | --- | --- | --- |
| AudioDriverKit | Develop drivers for audio devices. | DriverKit 21.0+ |  |  |  |
| BlockStorageDeviceDriverKit | Develop drivers for custom storage devices that communicate with the driver using custom protocols. | DriverKit 21.0+ |  |  |  |
| DriverKit | Develop device drivers that run in user space. | DriverKit 19.0+ | macOS 10.15+ | iOS 16.0+ | iPadOS 16.0+ |
| HIDDriverKit | Develop drivers for human-interface devices, such as keyboards, pointing devices, and digitizers like pens and touch pads. | DriverKit 19.0+ | macOS 10.15+ |  |  |
| MIDIDriverKit | Develop drivers for MIDI devices. | DriverKit 24.0+ |  |  |  |
| NetworkingDriverKit | Develop drivers for Ethernet networking devices. | DriverKit 19.0+ |  |  |  |
| PCIDriverKit | Develop device drivers for Peripheral Component Interconnect (PCI) accessories. | DriverKit 19.0+ | macOS 11.1+ |  |  |
| SCSIControllerDriverKit | Develop drivers for SCSI protocol-based devices. | DriverKit 20.4+ |  |  |  |
| SCSIPeripheralsDriverKit | Develop drivers for peripherals that use SCSI Block Command and Multimedia Command protocols. | DriverKit 22.0+ |  |  |  |
| SerialDriverKit | Develop drivers for serial I/O devices connected to your Mac. | DriverKit 19.0+ |  |  |  |
| USBDriverKit | Develop drivers for USB-based devices. | DriverKit 19.0+ |  |  |  |
| USBSerialDriverKit | Develop drivers for serial USB devices connected to your Mac. | DriverKit 19.0+ |  |  |  |

# Web

| Technology | <div style="width:290px">Description</div> | Framework |
| --- | --- | --- |
| Apple Pay on the Web | Support Apple Pay on your website with JavaScript-based APIs. | Safari Desktop 10.0+, Safari Mobile 10.0+ |
| CKTool JS | Manage your CloudKit containers and databases from JavaScript. | CKTool JS 1.2.15+ |
| CloudKit JS | Provide access from your web app to your CloudKit app’s containers and databases. | CloudKit JS 1.0+ |
| LivePhotosKit JS | Play Live Photos on the web. | LivePhotosKit JS 1.0+ |
| MapKit JS | Embed interactive Apple Maps on your website, annotate points of interest, and perform georelated searches. | MapKit JS 5.0+ |
| visionOS | Create a new universe of apps and games for Apple Vision Pro. | visionOS 1.0+ |
| WebKit JS | Access and modify DOM elements within a webpage, including touch events and visual effects. | Safari Desktop 9.0+, Safari Mobile 9.0+ |

# Others

| Title | <div style="width:290px">Description</div> | URL |
| --- | --- | --- |
| App License Delivery SDK | Secure the installation of alternative distribution apps on iOS or iPadOS devices by vending licenses from your web server. | https://developer.apple.com/documentation/AppLicenseDeliverySDK |
| Apple Pay Merchant Token Usage Information API | Add details about your merchant token usage information package. | https://developer.apple.com/documentation/ApplePayMerchantTokenUsageInformation |
| Apple Pencil | Enhance your iPad app’s user experience by supporting drawing, handwriting, and other features of Apple Pencil. |  |
| Apple silicon | Get the resources you need to create software for Macs with Apple silicon. | https://developer.apple.com/documentation/apple-silicon |
| Enterprise Program API | Automate the tasks you perform on the Apple Developer website. | https://developer.apple.com/documentation/EnterpriseProgramAPI |
| HTTP Live Streaming | Send audio and video to iOS, tvOS, and macOS devices. | https://developer.apple.com/documentation/HTTP-Live-Streaming |
| Human Interface Guidelines | The HIG contains guidance and best practices that can help you design a great experience for any Apple platform. | https://developer.apple.com/design/human-interface-guidelines/ |
| Mac Catalyst | Create a version of your iPad app that users can run on a Mac device. | https://developer.apple.com/documentation/UIKit/mac-catalyst |
| MusicKitJS | MusicKit on the Web brings Apple Music to your website — with songs, music videos, radio stations, and full access to the Apple Music API. And now with MusicKit Web Components, you can build richer integrations with less code, faster. | https://js-cdn.music.apple.com/musickit/v3/docs/index.html?path=/story/introduction--page |
| Professional Video Applications | Exchange data with Final Cut Pro, and create effects plug-ins for Final Cut Pro and Motion. |  |
| QuickTime File Format | An object-oriented file format for the storage and exchange of digital media between devices, applications, and operating systems. |  |
| Safari app extensions | Learn how Safari app extensions extend the web-browsing experience in Safari by leveraging web technologies and native code. |  |
| SecureElementCredential | Allow access to credentials inside the Secure Element on device. | https://developer.apple.com/documentation/SecureElementCredential |
| TVML | Use Apple TV Markup Language to create individual pages inside of a client-server app. | https://developer.apple.com/documentation/TVML |
| USD | An efficient and scalable way to represent 3D scenes. | https://developer.apple.com/documentation/USD |
| Vision | Apply computer vision algorithms to perform a variety of tasks on input images and videos. | https://developer.apple.com/documentation/Vision |
| visionOS | Create a new universe of apps and games for Apple Vision Pro. |  |
| watchOS apps | Build watchOS apps that combine complications, notifications, and Siri to create a personal experience on Apple Watch. | https://developer.apple.com/documentation/watchOS-Apps |