import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

// Stateless widget for overall app
class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return const MaterialApp(
      title: 'Layout Demo',
      home: LoginPage(), // Stateful widget used here
    );
  }
}

// Stateful widget for login page
class LoginPage extends StatefulWidget {
  const LoginPage({super.key});

  @override
  State<LoginPage> createState() => _LoginPageState();
}

class _LoginPageState extends State<LoginPage> {
  String username = '';
  String password = '';

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text('LOGIN PAGE'),
      ),
      body: Center(
        child: Container(
          height: 500.0,
          width: 400.0,
          padding: const EdgeInsets.all(20),
          decoration: BoxDecoration(
            color: Colors.yellow[100],
            borderRadius: BorderRadius.circular(16),
          ),
          child: Column(

            mainAxisAlignment: MainAxisAlignment.center,
            children: const [
              Text("LOGIN", style: TextStyle(fontSize: 30,decoration: TextDecoration.underline),),
              TextField(
                decoration: InputDecoration(
                  labelText: 'USER NAME',
                  icon: Icon(Icons.email_outlined),
                  border: OutlineInputBorder(),
                ),
              ),
              SizedBox(height: 20),
              TextField(
                obscureText: true,
                decoration: InputDecoration(
                  labelText: 'PASSWORD',
                  icon: Icon(Icons.password_outlined),
                  border: OutlineInputBorder(),
                ),
              ),
              SizedBox(height: 30),
              ElevatedButton(
                onPressed: null, // No functionality as requested
                child: Text('LOGIN'),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
