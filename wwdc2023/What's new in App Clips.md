# What's new in App Clips
## WWDC 2023
[What's new in App Clips][whats new in app clips]

---

New Improvements:
- New size limit
- Default App Clip links
- Invoke from your app

---

## New Size Limit

iOS 16 and above - 50 MB
iOS 15 and below - 10 MB

- allows for richer digital invocations
- enhance your App Clip functionality
- provide more immersive experience

---

## Default App Clip links
__Starting - iOS 16.4__

App Clip links are powered by Universal Links.

Invoked using universal link
```
https://naturelab.example.com/
```

For more, see: [Configure and link your App Clips: WWDC20][configure and link your app clips]


App Clip links are Apple generated URL when you publish an App Clips in AppStore Connect.
- Invokes default app clip experience

    ```
    https://appclip.apple.com/id?p=com.example.naturegarden.bakyardbirds.Clip
    ```

Link format:
```
https://appclip.apple.com/id?p=<bundle_id>&key=value    
```
where
- `bundle_id` is your App Clip bundle id.
- `key=value` is app specif parameters that can be retrieved in your app clip at launch.


For example, a game demo App Clip might use a parameter to know which character to use
```swift
ContentView(parameters: $parameters)
 .onContinueUserActivity(NSUserActivityTypeBrowsingWeb, perform: { userActivity in
   guard let inputURL = userActivity.webpageURL else {
    return
   }

   let component = NSURLComponents(url: inputURL, resolvingAgainstBaseURL: true)
   guard let parameters = components?.queryItems else {
    return
   }

   self.parameters = parameters

 })
```


---

## Invoke from your app
__Starting - iOS 17__

1. Invoke your App Clip from any application.

    ```swift
    // use link presentation API to generate a tappable rich preview of the App Clip that will aloow it to be invoked

    let lpView: LPLinkView = ...
    let provider = LPMetadataProvider()
    provider.startFetchingMetadata(for: url) { (metadata, error) in
        guard let metadata = metadata else {
        return
        }

        DispatchQueue.main.async {
        // once you've retrieved the metadata using LPMetadataProvider
        // you can pass it to LPLinkView to render a preview.
        lpView.metadata = metadata
        }
    }
    ```

2. If your app uses default App Clip links:
    
   you can invoke it directly

   ```swift
   // Launching App Clips from your app

   var body: some View {
    let appClipURL = URL(
        string: "https://appclip.apple.com/id?p=com.example.naturelab.backyardbirds.Clip"
    )!

    Link("Backyard Birds", destination: appClipURL)
   }
   ```
   or call open on UIApplication
   ```swift
   // Launching App Clips from your app

   func launcAppClip {
    let appClipURL = URL(
        string: "https://appclip.apple.com/id?p=com.example.naturelab.backyardbirds.Clip"
    )!

    UIApplication.shared.open(appClipURL)
   }
   ```
---

## Wrap-up

- Build richer App Clip experiences
- Set up easily with default App Clip links
- Launch App Clips from your app.

---

## Reference
- [What's new in App Clips][whats new in app clips]
- [Configure and link your App Clips: WWDC20][configure and link your app clips]


[whats new in app clips]: https://developer.apple.com/videos/play/wwdc2023/10178/
[configure and link your app clips]: https://developer.apple.com/videos/play/wwdc2020/10146/
