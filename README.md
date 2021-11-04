# flutter_file_picker_1

https://pub.dev/packages/file_picker

file_picker: ^4.2.0

check https://github.com/miguelpruivo/flutter_file_picker/wiki/Setup

https://pub.dev/packages/open_file

open_file: ^3.2.1

Programm selektiert eine Datei auf Android und IOS

Nachteil: die Datei wird gecached (intern kopiert)

Basis: https://protocoderspoint.com/flutter-file_picker-package-pick-image-video-doc-file-picker-example/

Youtube: https://www.youtube.com/watch?v=GkjbimwxsWM

https://stackoverflow.com/questions/53296899/how-to-clear-app-cache-programmatically-on-flutter/54268590

oder in https://www.codegrepper.com/code-examples/dart/flutter+clear+cache+programmatically

Löschung des Cashes und des AppDir Verzeichnisses

import 'package:path_provider/path_provider.dart';
Future<void> _deleteCacheDir() async {
final cacheDir = await getTemporaryDirectory();
if (cacheDir.existsSync()) {
cacheDir.deleteSync(recursive: true);}}
// achtung: dieser teil löscht das appdir verzeichnis
final appDir = await getApplicationSupportDirectory();
if (appDir.existsSync()) {
appDir.deleteSync(recursive: true);}}




A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
