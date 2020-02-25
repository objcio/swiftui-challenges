Your challenge is to align a `VStack` of `HStack`s in such a way that it displays as two columns:

```swift
VStack {
    HStack {
        Text("100 m").font(Font.body.bold())
        Text("Usain Bolt")
    }
    HStack {
        Text("5 km").font(Font.body.bold())
        Text("Joshua Cheptegei")
    }
    HStack {
        Text("10 km").font(Font.body.bold())
        Text("Rhonex Kipruto")
    }
    HStack {
        Text("Marathon").font(Font.body.bold())
        Text("Eliud Kipchoge")
    }
}
```

Try to achieve this using alignment guides, not using preferences. Of course both columns should adapt to the width of the contents.
