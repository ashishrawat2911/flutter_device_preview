# flutter_device_preview (WIP)

![gif](https://github.com/aloisdeniel/flutter_device_preview/raw/master/device_preview.gif)

Preview of your app on various device screen configurations from one of your devices and save time when adapting your app visuals for various form factors.

Targeted features :

* Preview any device from any device
* Change Device orientation
* Display a device frames 
* Change the device at any time but keep the application state
* Take screenshots

## Quickstart

```dart
void main() => runApp(
  DevicePreview(
    child: MyApp(),
  ),
);
```


```dart
class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      builder: DevicePreview.appBuilder, // <--- Add the builder 
      title: 'Flutter Demo',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: MyHomePage(title: 'Flutter Demo Home Page'),
    );
  }
}
```

## Roadmap

[ ] Show/Hide frame
[ ] Android devices
[ ] Desktop devices
[ ] TV devices
[ ] Orientations
[ ] Screenshot (share, mode)
[ ] Documentation
[ ] Clean code