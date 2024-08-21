# fancy_container_update

A new Flutter package project.
## Features

 - user can make fancy type container
 - easy and simple decoration

## Getting started

To use this package, add text_scroll as a dependency in your pubspec.yaml file.

## Usage

Minimal example:
```add dependeces
  new_fancy_flutter_container: ^0.0.5
```

```import
    import 'package:new_fancy_flutter_container/fancy_container.dart';
```

Custom settings:

```dart
   import 'package:flutter/material.dart';
import 'package:new_fancy_flutter_container/fancy_container.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      title: 'Flutter Demo',
      theme: ThemeData(
        colorScheme: ColorScheme.fromSeed(seedColor: Colors.deepPurple),
        useMaterial3: true,
      ),
      home: myHome(),
    );
  }
}

class myHome extends StatefulWidget {
  const myHome({super.key});

  @override
  State<myHome> createState() => _myHomeState();
}

class _myHomeState extends State<myHome> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: FancyContainer(
        height: MediaQuery.of(context).size.height / 2,
        color1: Colors.amber,
        color2: Colors.black,
        width: MediaQuery.of(context).size.width,
        child: Center(
          child: Text(
            "data",
            style: TextStyle(
                color: Colors.white, fontSize: 40, fontWeight: FontWeight.w600),
          ),
        ),
      ),
    );
  }
}

```
