 # SoftEdgeBlur

A Flutter widget that applies a soft, blurred edge effect to its child widget. This package allows you to easily add a subtle, fading blur effect to the top and/or bottom edges of any widget, creating a smooth transition between content and background.

<img width="547" alt="Screenshot 2024-09-10 at 23 04 14" src="https://github.com/user-attachments/assets/ba58e8a7-a499-46b0-8f41-6eb74dfb8738">


## Getting Started

To use this package, add `soft_edge_blur` as a dependency in your `pubspec.yaml` file.

```yaml
dependencies:
  soft_edge_blur: 
```

Then, run:

```
flutter pub get
```

## Usage

Import the package in your Dart code:

```dart
import 'package:soft_edge_blur/soft_edge_blur.dart';
```

Wrap any widget with `SoftEdgeBlur` to apply the blur effect:

```dart
SoftEdgeBlur(
  edges: [
    EdgeBlur(EdgeType.topEdge, 20, 3),
  ],
  child: YourWidget(),
)
```

### Parameters

- `edges`: A list of `EdgeBlur` objects defining which edges to blur and their properties.
- `child`: The widget to which the blur effect will be applied.

Each `EdgeBlur` object takes three parameters:
1. `EdgeType`: Either `EdgeType.topEdge` or `EdgeType.bottomEdge`
2. `size`: The size of the blurred area in logical pixels
3. `sigma`: The intensity of the blur effect


## Demo

Check out this video to see `SoftEdgeBlur` in action:




https://github.com/user-attachments/assets/e42d79ab-657d-4a1b-90be-5fbd44f1a957


