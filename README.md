# ionic-custom-font
Use of custom font in Ionic app

A simple example of using custom fonts in Ionic application.

## Run this sample application
1. git clone https://github.com/varnit-abraham/ionic-custom-font.git
1. cd ionic-custom-font
1. npm install
1. ionic cordova prepare android
1. ionic cordova emulate android (on emulator) or ionic cordova run android (on device)

## Environment details
cli packages: (C:\Users\varni\AppData\Roaming\npm\node_modules)

    @ionic/cli-utils  : 1.19.1
    ionic (Ionic CLI) : 3.19.1

global packages:

    cordova (Cordova CLI) : 6.5.0

local packages:

    @ionic/app-scripts : 3.1.8
    Cordova Platforms  : android 6.1.2
    Ionic Framework    : ionic-angular 3.9.2

System:

    Android SDK Tools : 25.2.3
    Node              : v8.9.1
    npm               : 5.6.0
    OS                : Windows 10

## Custom Fonts used
1. [dacasa](https://www.urbanfonts.com/fonts/da_Casa.font)
1. [Ageng Sans](https://www.urbanfonts.com/fonts/Ageng_Sans.font)

## Steps to include custom fonts
1. Add custom font to your `src/assets/fonts` folder.
1. Add font family definition to use in variables.scss file
    ```
    @font-face {
      font-family: "dacasa";
      src: url("../assets/fonts/dacasa.ttf")
    }
    ```
1. To change the default font family being used in the app, add below line to variables.scss file.
    ```
    *{
      font-family: "dacasa";
    }
    ```
1. To apply any custom font to any element via css, add below code in your .scss file
    ```
    .cus_font {
        font-family:    Ageng Sans;
        font-size:      40px;
        font-weight:    bold;
    }
    
    <element class="cus_font"></element>
    ```
    
    
   
