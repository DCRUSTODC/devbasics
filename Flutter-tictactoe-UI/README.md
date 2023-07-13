# TicTacToe
## Flutter
It is a UI framework built by Google. It can be used to create 
1. Android Application
2. Ios Application
3. Windows Application 
4. MacOs Application
5. Linux Application 

These are the officially mentioned applications that can be build using flutter. Although flutter can be used to create applications for any OS and can even connect it to Rasberry pi \
It uses Dart language as it is made specially for handling client side services. 
Dart language can be seen as a hybrid of other modern day languages in the way that
1. It supports the dynamic variables using var and dyanmic keyword but also supports the static data type declaration by Java type convention,
2. It also supports the async await keywords of JavaScript and the promises of JavaScript are referred as Future<> type.
3. It is OOP language supporting single inheritance but also supports features like multi mixins usage in classes and interfaces.
4. It supports keywords like assert and yield in python.

You can explore Dart on the official [website](https://dart.dev/guides)

Lets jump to create our first project. \
We will directly start from the coding part. You can install flutter sdk from [here](https://docs.flutter.dev/get-started/install) and follow the steps shown for completing the setup.
- Create a Project Using the following command\
 `flutter create tictactoe` \
 This command creates a basic counter application in flutter as a demonstration. If you have created an android emulator. \
 Go to android studio and create one if not already created and start the emulator.\
 Follow the command at the root of the applicaton created to run the application in the emulator
 ```
 cd tictactoe
 flutter run
 ```
 This command builds the application in debug mode and and install in the current running adroid emulator. \
 If no emulator is running, it shows options to run the application in the web and in the desktop. (But you should have already installed all the dependencies for application development for different OS)
- Open the project in Vs Code or Android Studio. Follow the command to open the project in Vs Code\
 `code .` \
 At the root level of project
- Go to to `main.dart` in the `tictactoe/lib` . This is the root file of your project. `lib` folder contains all the widget related code of your project.
- Create folders `widgets` and `screens` in the `lib` folder. All the screens should have a seperate folder by convention and the custom widgets should fall in the `widgets` folder by further nested folders naming screens.
```
widgets/
  global_widget1.dart
  global_widget2.dart
  etc.dart
  home/ 
    my_button.dart
    my_list_tile.dart
  auth/
    login_button.dart
    signup_button.dart
 ```
This convention should be followed for your project.
- Create `home_screen.dart` in the `screens` folder. On this screen, you can give the the user to choose who's going to have the first turn.\
To implement this you can use either a `Row` or a `Column` widget in the center of the screen using `Center` widget. Use the `IconButton` widget as the children of `Row` or `Column` for indicating the turns.
- Create `player_screen.dart` in the same folder. In this screen implement the game board using the `GridView` widget.
- Create a `functions` folder in the `lib` folder. Implement the logic of the game in a separate class so that you can manage it on both the screens.
- Connect both the screens using `Navigator` in the ontap method of the `IconButton` widgets.
- Give some colors and decorations to your app.

Hint : Flutter's devtools and editor's docs are very powerful for devlopers, use them wisely.

There are thousands of other widgets available in flutter which you can use in your application. Go check out at [flutter Docs](https://docs.flutter.dev/).
