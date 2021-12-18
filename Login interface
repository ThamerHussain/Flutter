import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      theme: ThemeData(primarySwatch: Colors.lightBlue),
      home: textfield(),
    );
  }
}


class textfield extends StatefulWidget {
  @override
  State<StatefulWidget> createState() => _textfieldss();
}

class _textfieldss extends State<textfield> {
  bool obscure = true;
  bool bar = true;
  var visIcon = Icons.visibility_off;
  var wc = Colors.white;
  var bc = Colors.black;
  var str = "Age";
  late int birth_year;
  int Age_year = 0;
  var age_text = "";
  //var c = Colors.white;
  //var wc = Colors.white;
  var mycontroller = TextEditingController();
  var controllermy = TextEditingController();
  var textcolor = Colors.teal;
  var iconscolor = Colors.pink;
  var lb = Colors.lightBlue[300];
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: bar ? wc : bc,
      appBar: AppBar(
        centerTitle: true,
        title: const Text("Flutter with Thamer"),
        backgroundColor: Colors.indigoAccent,
      ),
      body: Container(
        //color: Colors.black87,
        height: double.infinity,
        margin: const EdgeInsets.all(100.0),
        child: SingleChildScrollView(
          child: Column(
            children: <Widget>[
              const SizedBox(height: 30),
              Container(
                padding: const EdgeInsets.all(1.0),
                margin: const EdgeInsets.all(1.0),
                child: TextField(
                  controller: controllermy,
                  decoration: InputDecoration(
                      suffixIcon: IconButton(
                          onPressed: () {
                            setState(() {
                              birth_year = int.parse(controllermy.text);
                            });
                            Age_year = DateTime.now().year - birth_year;
                            age_text = "your age is $Age_year years old";
                          },
                          icon: const Icon(Icons.bug_report)),
                      labelText: str,
                      hintText: "Enter your birth year",
                      labelStyle: TextStyle(
                        fontSize: 20,
                        color: textcolor,
                      ),
                      icon: Icon(
                        Icons.format_color_text_outlined,
                        color: iconscolor,
                      )),
                ),
              ),
              Container(
                  padding: const EdgeInsets.all(1.0),
                  margin: const EdgeInsets.all(1.0),
                  child: Text(
                    age_text,
                    style: const TextStyle(height: 2),
                  )),
              Container(
                padding: const EdgeInsets.all(1.0),
                margin: const EdgeInsets.all(1.0),
                child: TextField(
                  decoration: InputDecoration(
                      /*filled: true,
                      fillColor: Colors.blueGrey[900],
                      enabledBorder: OutlineInputBorder(
                          borderRadius: BorderRadius.circular(27.1),
                          borderSide: const BorderSide(
                            width: 0.2,
                            color: Colors.white,
                          )),*/
                      labelText: "Name",
                      labelStyle: TextStyle(
                        fontSize: 20,
                        color: textcolor,
                      ),
                      hintText: "Enter the Name",
                      hintStyle: TextStyle(
                        fontSize: 19,
                        color: lb,
                      ),
                      icon: Icon(
                        Icons.person,
                        color: iconscolor,
                      )),
                  maxLines: 2,
                  style: TextStyle(color: bar ? bc : wc),
                  keyboardType: TextInputType.text,
                ),
              ),
              Container(
                padding: const EdgeInsets.all(1.0),
                margin: const EdgeInsets.all(1.0),
                child: TextField(
                  decoration: InputDecoration(
                      /*filled: true,
                      fillColor: Colors.blueGrey[900],
                      enabledBorder: OutlineInputBorder(
                          borderRadius: BorderRadius.circular(27.1),
                          borderSide: const BorderSide(
                            width: 0.2,
                            color: Colors.white,
                          )),*/
                      labelText: "Email",
                      labelStyle: TextStyle(
                        fontSize: 20,
                        color: textcolor,
                      ),
                      hintText: "Enter the Email",
                      hintStyle: TextStyle(
                        fontSize: 19,
                        color: lb,
                      ),
                      icon: Icon(
                        Icons.email,
                        color: iconscolor,
                      )),
                  style: TextStyle(color: bar ? bc : wc),
                  keyboardType: TextInputType.emailAddress,
                ),
              ),
              Container(
                padding: const EdgeInsets.all(1.0),
                margin: const EdgeInsets.all(1.0),
                child: TextField(
                  decoration: InputDecoration(
                    /*filled: true,
                      fillColor: Colors.blueGrey[900],
                      enabledBorder: OutlineInputBorder(
                          borderRadius: BorderRadius.circular(27.1),
                          borderSide: const BorderSide(
                            width: 0.2,
                            color: Colors.white,
                          )),*/
                    labelText: "Password",
                    labelStyle: TextStyle(
                      fontSize: 20,
                      color: textcolor,
                    ),
                    hintText: "Enter the Password",
                    hintStyle: TextStyle(
                      fontSize: 19,
                      color: lb,
                    ),
                    icon: Icon(
                      Icons.password,
                      color: iconscolor,
                    ),
                    //prefixIcon: Icon(Icons.disabled_by_default_rounded),
                    suffixIcon: IconButton(
                      icon: Icon(
                        obscure ? Icons.visibility_off : Icons.visibility,
                      ),
                      onPressed: () {
                        setState(() {
                          obscure = !obscure;
                        });
                      },
                      color: Colors.purple,
                    ),
                  ),
                  style: TextStyle(color: bar ? bc : wc),
                  keyboardType: TextInputType.visiblePassword,
                  obscureText: obscure,
                ),
              ),
              Container(
                padding: const EdgeInsets.all(1.0),
                margin: const EdgeInsets.all(1.0),
                child: TextField(
                  decoration: InputDecoration(
                      /*filled: true,
                      fillColor: Colors.blueGrey[900],
                      enabledBorder: OutlineInputBorder(
                          borderRadius: BorderRadius.circular(27.1),
                          borderSide: const BorderSide(
                            width: 0.2,
                            color: Colors.white,
                          )),*/
                      prefixText: "+964 ",
                      //suffixText: "",
                      labelText: "Number",
                      labelStyle: TextStyle(
                        fontSize: 20,
                        color: textcolor,
                      ),
                      hintText: "Enter the Number",
                      hintStyle: TextStyle(
                        fontSize: 19,
                        color: lb,
                      ),
                      icon: Icon(
                        Icons.phone,
                        color: iconscolor,
                      )),
                  style: TextStyle(color: bar ? bc : wc),
                  keyboardType: TextInputType.number,
                  controller: mycontroller,
                ),
              ),
              Container(
                padding: const EdgeInsets.all(1.0),
                margin: const EdgeInsets.all(1.0),
                child: ElevatedButton(
                    onPressed: () => setState(() {
                          str = mycontroller.text;
                        }),
                    style: ButtonStyle(
                        foregroundColor:
                            MaterialStateProperty.all(bar ? wc : bc),
                        backgroundColor:
                            MaterialStateProperty.all(Colors.pink)),
                    child: const Padding(
                      padding: EdgeInsets.fromLTRB(30, 10, 30, 10),
                      child: Text(
                        "get value",
                        style: TextStyle(fontSize: 23),
                      ),
                    )),
              ),
              const SizedBox(height: 30),
            ],
          ),
        ),
      ),
      floatingActionButton: FloatingActionButton(
        child: Icon(
          Icons.mode_night_rounded,
          color: bar ? bc : wc,
        ),
        backgroundColor: bar ? wc : bc,
        onPressed: () => setState(() {
          bar = !bar;
        }),
      ),
      floatingActionButtonLocation: FloatingActionButtonLocation.miniStartFloat,
    );
  }
}
