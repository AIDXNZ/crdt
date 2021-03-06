Dart implementation of Conflict-free Replicated Data Types (CRDTs).

This project is heavily influenced by James Long's talk [CRTDs for Mortals](https://www.dotconferences.com/2019/12/james-long-crdts-for-mortals) and includes a Dart-native implementation of Hybrid Local Clocks (HLC) based the paper [Logical Physical Clocks and Consistent Snapshots in Globally Distributed Databases](https://cse.buffalo.edu/tech-reports/2014-04.pdf).

It has [zero external dependencies](https://github.com/cachapa/crdt/blob/master/pubspec.yaml), so it should run everywhere where Dart runs.

## Usage

The `Crdt` class works as a layer on top of a map. The simplest way to experiment is to initialise it an empty map:

```dart
import 'package:crdt/crdt.dart';

main() {
  var crdt = Crtd.fromMap({});
}
```

You'll probably want to can implement [Store](https://github.com/cachapa/crdt/blob/master/lib/src/store.dart) if you want to offer any sort of persistence though.

## Features and bugs

Please file feature requests and bugs at the [issue tracker](https://github.com/cachapa/crdt/issues).
