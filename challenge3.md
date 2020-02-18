Your challenge is to create a tab-bar like component that has a smooth animation:

<https://github.com/objcio/swiftui-challenges/blob/master/challenge3.mov?raw=true>

This is the interface we expect:

```swift
struct TabBar: View {
    var items: [(Image, Text)]
    @State var selectedIndex: Int = 0
    var body: some View {
        fatalError("TODO")
    }
}
```

That means you should be able to replicate the tab bar in the movie above using the following code:

```swift
struct ContentView: View {
    var body: some View {
        return TabBar(items: [
            (Image(systemName: "tray"), Text("Inbox")),
            (Image(systemName: "archivebox"), Text("Archive")),
            (Image(systemName: "doc.text"), Text("Drafts"))
        ]).padding().border(Color.blue)
    }
}
```
