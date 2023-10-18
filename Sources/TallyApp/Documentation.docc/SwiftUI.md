# SwiftUI
SwiftUI helps you build great-looking apps across all Apple platforms with the power of Swift — and surprisingly little code. You can bring even better experiences to everyone, on any Apple device, using just one set of tools and APIs.

![](hero-lockup-swiftui-large_2x.png)

## Declarative syntax

SwiftUI uses a declarative syntax, so you can simply state what your user interface should do. For example, you can write that you want a list of items consisting of text fields, then describe alignment, font, and color for each field. Your code is simpler and easier to read than ever before, saving you time and maintenance.


```swift
import SwiftUI

struct AlbumDetail: View {
    var album: Album

    var body: some View {
        List(album.songs) { song in 
            HStack {
                Image(album.cover)
                VStack(alignment: .leading) {
                    Text(song.title)
                    Text(song.artist.name)
                        .foregroundStyle(.secondary)
                }
            }
        }
    }
}
```

This declarative style even applies to complex concepts like animation. Easily add animation to almost any control and choose a collection of ready-to-use effects with only a few lines of code. At runtime, the system handles all of the steps needed to create a smooth movement, even dealing with user interaction and state changes mid-animation. With animation this easy, you’ll be looking for new ways to make your app come alive.

## Design tools
Xcode includes intuitive design tools that make it easy to build interfaces with SwiftUI. As you work in the design canvas, everything you edit is completely in sync with the code in the adjoining editor. Code is instantly visible as a preview as you type and you can even view your UI in multiple configurations, such as light and dark appearance. Xcode recompiles your changes instantly and inserts them into a running version of your app — visible, and editable at all times.

![](example-design-large_2x.png)

**Dynamic replacement**. The Swift compiler and runtime are fully embedded throughout Xcode, so your app is constantly being built and run. The design canvas you see isn’t just an approximation of your user interface — it’s your live app. And Xcode can swap edited code directly in your live app using dynamic replacement.
Previews. You can now create one or many previews of any SwiftUI views to get sample data, and configure almost anything your users might see, such as large fonts, localizations, or Dark Mode. Previews can also display your UI in any device and any orientation.

## Works with UIKit and AppKit
SwiftUI is designed to work alongside UIKit and AppKit, so you can adopt it incrementally in your existing apps. When it’s time to construct a new part of your user interface or rebuild an existing one, you can use SwiftUI while keeping the rest of your codebase.
And if you want to use an interface element that isn’t offered in SwiftUI, you can mix and match SwiftUI with UIKit and AppKit to take advantage of the best of all worlds.
