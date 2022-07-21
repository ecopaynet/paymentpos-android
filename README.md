# PaymentPOS module for Android
The PaymentPOS module facilitates the communication between your application and the payment device served by Ecopaynet. Fast, easy and powerful.

You only need to worry about the amount of the transaction, the rest of the work is made by the module.

PaymentPOS communicates with TCP, Bluetooth and Serial Port payment devices served by Ecopaynet. This devices are robust, secure and certified to make card payments using contactless, NFC, chip, magnetic stripe and manual input.

## Requirements
- Android minimum SDK version 16 (4.1 Jelly Bean)
 
## Dependencies
PaymentPOS uses kotlin internally so the following dependencies are required to work:
 - org.jetbrains.kotlinx:kotlinx-coroutines-android (implementation)
 - org.jetbrains.kotlinx:kotlinx-datetime (implementation)
 - org.jetbrains.kotlinx:kotlinx-serialization-json (implementation)
 - androidx.constraintlayout:constraintlayout (implementation)
 - io.ktor:ktor-client-android (implementation)
 - io.ktor:ktor-client-content-negotiation (implementation)
 - io.ktor:ktor-serialization-kotlinx-json (implementation)

## Installation
PaymentPOS comes in an Android Java Library (AAR) format. We recommend the use of the Android Studio IDE.

Steps to integrate it on your Android Studio project:
 1. Open your Android Studio project	
 2. Copy the AAR file into the "libs" folder of your project (normally in /app/libs)
 3. Open the project's gradle file
 4. Add "\*.aar" in the fileTree implementation line, next to "\*.jar". 
 5. Add the latest versions of the dependencies..

Once this steps are done and Gradle Sync has finished, you will be able to call any method of the PaymentPOS module.

## Java 8 compatibility
Since the module uses Java 8 methods, you probably have to make your project compatible with the following steps. This process is called *"desugaring"*.
 1. Add "multiDexEnabled true" inside defaultConfig.
 2. Add "coreLibraryDesugaringEnabled true" inside compileOptions.
 3. Add dependency com.android.tools:desugar_jdk_libs (coreLibraryDesugaring)
	
## Getting Started
See our [Android PaymentPOS Getting Started](https://github.com/ecopaynet/Android-PaymentPOS-Getting-Started) project to see the module in action.
 
## License
PaymentPOS is copyright of [Ecopaynet SL](https://www.ecopaynet.com)