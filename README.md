# font_awesome_flutter

The [Font Awesome](http://fontawesome.io/icons/) Icon pack available as set of Flutter Icons.

Based on Font Awesome 5.5. Includes all free icons:

  * Regular
  * Solid
  * Brands

## Installation

In the `dependencies:` section of your `pubspec.yaml`, add the following line:

```yaml
  font_awesome_flutter: <latest_version>
```

## Usage

```dart
import 'package:font_awesome_flutter/font_awesome_flutter.dart';

class MyWidget extends StatelessWidget {
  Widget build(BuildContext context) {
    return new IconButton(
      // Use the FontAwesomeIcons class for the IconData
      icon: new Icon(FontAwesomeIcons.gamepad), 
      onPressed: () { print("Pressed"); }
     );
  }
}
```

## Example

View the Flutter app in the `example` directory to see all the available `FontAwesomeIcons`.

## Include pro icons

If you bought font awesome pro icons, you can import them here. 

:exclamation: By importing pro icons you acknowledge that it is your obligation to keep these files private. This includes **not** uploading your package to github or other public file sharing services.

- [Download this package's source](https://github.com/michaelspiss/font_awesome_flutter/archive/master.zip), extract the folder and move it to a location of your choice
- In your project's dependencies, replace the version tag for `font_awesome_flutter` with the path to your custom installation:
```yaml
dependencies:
  font_awesome_flutter:
    path: /path/to/font_awesome_flutter
    ...
```
- Remove `#`s from `pubspec.yaml` at the indicated position
- Run `pub get`
- Download your font awesome pro icons (web version)
- Move all `.ttf` files from the `webfonts` directory to this package's lib/fonts (replace existing fonts)
- Move `icons.json` from `metadata` to this directory (package root)
- Run `./tool/update.sh` (from this package's root)

## Contributors

  - Brian Egan
  - Phil Plante
