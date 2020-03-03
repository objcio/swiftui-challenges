Your challenge is to animate a line. Here's the code that draws a line using a simple path:

```swift
let p1 = CGPoint(x: 50, y: 50)
let p2 = CGPoint(x: 100, y: 25)
let p3 = CGPoint(x: 100, y: 100)

struct ContentView: View {
    @State var toggle = true
    var body: some View {
        VStack {
            Button("Toggle") {
                withAnimation(.default) {
                    self.toggle.toggle()
                }
            }
            Path { p in
                p.move(to: toggle ? p1 : p2)
                p.addLine(to: p3)
            }.stroke(lineWidth: 2)
          
        }
    }
}
```

Currently, the line doesn't animate to its new position. Wrap the `Path` in a `Shape` and make sure the start and end points of the line are animatable.
