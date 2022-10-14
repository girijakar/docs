---
Title: 'Button'
Description: 'A very basic component in UI, which is used to interact and perform certain actions'
Subjects:
  - 'Sotfware Development'
  - 'Mobile Development'
  - 'Computer Science'
Tags:
  - 'SwiftUI'
  - 'SwiftUI Views'
  - 'Buttons'
  - 'Views'
CatalogContent:
  - 'learn-swiftui'
  - 'paths/build-ios-apps-with-swiftui'
---

A very basic component in UI, which is used to interact and perform certain actions, such as logging into a page, or deleting a file etc.

## Syntax

```psuedo
Button("Text inside the button"){
  //What happens when you click the button
}
```

The `Text inside the button` is what is shown inside the button.

## Example

To make a button which `count` the number of times we `click` it:


```swift
@State var count = 0
var body: some View {
  Button("Click me: \(count)") {
     self.count += 1
  }
 .font(.title)
 .padding()
 .backgroundColor(Color.green)
 .cornerRadius(40)
 .foregroundColor(Color.black)
 .overlay(RoundedRectangle(cornerRadius: 40).stroke(Color.green))
```
This will display the following:

![Button](https://raw.githubusercontent.com/girijakar/docs/main/media/button.png)
