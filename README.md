# MultiTouchKit
=============

MultiTouchKit is a Swift package that provides a UIView subclass capable of handling multiple gestures at the same time. It allows users to interact with your app in new ways by detecting additional touches while panning and recognizing taps during a long press.

The package also includes functionality for natural movement of a UIView using pinch and pan gestures. With MultiTouchKit, you can create intuitive user interfaces that respond seamlessly to user input.

Features
--------

*   Supports multiple gestures simultaneously
*   Counts additional touches while panning
*   Detects taps during long press
*   Includes functionality for natural movement using pinch and pan gestures

Usage
-----

To use MultiTouchKit, simply add it to your project and initialize the `MultiTouchView` class. Then, add it to your view hierarchy and start listening for gestures.

swift

```swift
let multiTouchView = MultiTouchView(frame: CGRect(x: 0, y: 0, width: 100, height: 100))
view.addSubview(multiTouchView)

multiTouchView.didPan = { touches, state in
    // Handle pan gesture
}

multiTouchView.didPinch = { scale, state in
    // Handle pinch gesture
}

multiTouchView.didLongPress = { touch, state in
    // Handle long press gesture
}
```

Requirements
------------

*   iOS 11.0+
*   Xcode 11.0+
*   Swift 5.0+

Installation
------------

### Swift Package Manager

You can use the Swift Package Manager to install MultiTouchKit. Simply add the following line to your `Package.swift` file:

swift

```swift
.package(url: "https://github.com/example/MultiTouchKit.git", .upToNextMajor(from: "1.0.0")),
```

License
-------

MultiTouchKit is available under the MIT license. See the [LICENSE](LICENSE) file for more info.

We hope this package helps you create powerful and intuitive user interfaces for your app! If you have any questions or feedback, feel free to reach out to us.

---
