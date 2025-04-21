import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: AlignContainerDemo(),
 );
 }
}
class AlignContainerDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('Container with Alignment')),
 body: Center(
 child: Container(
 height: 150,
 width: 150,
 color: Colors.teal,
 alignment: Alignment.bottomRight, // ⬅️ Aligns child inside 
the container
 child: Text(
 'Bottom Right',
 style: TextStyle(color: Colors.white),
 ),
 ),
 ),
 );
 }
}
