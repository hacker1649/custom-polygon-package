
# Custom Polygon Package

A Flutter package for custom painting.

In this version of the Flutter package, we implemented a code that defines a widget named as `CustomPolygonWidget` that allows users to interactively adjust the number of sides, size, and rotation of a polygon using sliders. The also implemented a class named as `ShapePainter` that uses the provided parameters to draw the polygon on the canvas.

Additionally, we prepared the package for publishing on pub.dev, including setting up the necessary metadata and documentation.

## Installation 

1. Use this package as a library, Run this command:

✔️ With Dart:

```bash
$ dart pub add custom_polygon_package
```

✔️ With Flutter:

```bash
$ flutter pub add custom_polygon_package
```

2. This will add a line like this to your package's pubspec.yaml (and run an implicit `dart pub get`):

```yaml
dependencies:
  custom_polygon_package: ^0.0.1
```

3. Now in your Dart code, you can use:

```dart
import 'package:custom_polygon_package/custom_polygon_package.dart';
```

## Usage

<table>
<tr>
<td>

```dart
import 'package:flutter/material.dart';
import 'package:custom_polygon_package/custom_polygon_package.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Polygon Package Testing...',
      debugShowCheckedModeBanner: false,
      theme: ThemeData(
        colorScheme: ColorScheme.fromSeed(seedColor: Colors.deepPurple),
        useMaterial3: true,
      ),
      home: HomeScreen(),
    );
  }
}

class HomeScreen extends StatelessWidget {
  const HomeScreen({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Polygons', style: TextStyle(fontWeight: FontWeight.bold)),
        backgroundColor: Theme.of(context).colorScheme.inversePrimary,
      ),
      body: Center(
        child: CustomPolygonWidget(),
      ),
    );
  }
}
```

</td>
<td>
<img  src="https://github.com/hacker1649/custom-polygon-package/assets/88313681/6e6389c6-1728-4025-96ce-df79c5b3a885"  alt="">
</td>
</tr>
</table>

## Resources

1. [Creating Packages](https://dart.dev/guides/libraries/create-packages)

2. [Publishing Packages](https://dart.dev/tools/pub/publishing)

3. [How to draw and animate designs with Flutter CustomPaint Widget](https://blog.codemagic.io/flutter-custom-painter/)

4. [CustomPaint Class](https://api.flutter.dev/flutter/widgets/CustomPaint-class.html)

5. [CustomPainter Class](https://api.flutter.dev/flutter/rendering/CustomPainter-class.html)
