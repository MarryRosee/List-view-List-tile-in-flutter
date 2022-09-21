# List-view-List-tile-in-flutter
List-view-List-tile-in-flutter
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  // This widget is the root of your application.
  List list = [
    "ist",
    "2nd",
    "third",
    "fourth",
    "five",
    "six",
    "seven",
    "eight"
  ];
  List name = [
    "Mobile App developer",
    "UIUX DESIGNER",
    "WORDPRESS CUSTOMIZ",
    "GRAPHIC DESIGNER",
    "WHITEBOARD ANIMATOR",
    "Mobile App developer",
    "UIUX DESIGNER",
    "WORDPRESS CUSTOMIZ",
    "GRAPHIC DESIGNER",
    "WHITEBOARD ANIMATOR",
    "Mobile App developer",
    "UIUX DESIGNER",
    "WORDPRESS CUSTOMIZ",
    "GRAPHIC DESIGNER",
    "WHITEBOARD ANIMATOR",
    "Mobile App developer",
    "UIUX DESIGNER",
    "WORDPRESS CUSTOMIZ",
    "GRAPHIC DESIGNER",
    "WHITEBOARD ANIMATOR"
  ];
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      darkTheme: ThemeData(backgroundColor: Colors.pink),
      home: Scaffold(
        backgroundColor: Colors.green,
        appBar: AppBar(
          leading: Icon(
            Icons.menu,
            size: 40,
            color: Colors.deepOrange,
          ),
          actions: [
            Icon(
              Icons.shopping_bag_rounded,
              size: 40,
              color: Colors.blue,
            ),
          ],
          elevation: 36,
          backgroundColor: Colors.black,
          toolbarHeight: 70,
          centerTitle: true,
          title: Text(
            "Boutique",
            style: TextStyle(
                fontFamily: "cursive",
                fontStyle: FontStyle.italic,
                fontWeight: FontWeight.bold,
                fontSize: 30),
          ),
        ),
        body: Material(
          color: Colors.green,
          child: ListView.builder(
              itemCount: 20,
              itemBuilder: (BuildContext context, int item) {
                return ListTile(
                  leading: Icon(Icons.account_circle),
                  trailing: Icon(Icons.add),
                  title: Text("maryam"),
                  subtitle: Text(name[item]),
                );
              }),
        ),
      ),
    );

    // Application name
  }
}
