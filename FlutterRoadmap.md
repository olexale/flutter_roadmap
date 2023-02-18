# Highly Subjective Roadmap to Flutter Development
by Oleksandr Leushchenko (@olexale)


## Basics
### Dev Environment

* Android Studio or Visual Studio Code (Must have)
* Flutter CLI (Nice to have)
* Git (Nice to have)
* DartPad (Optional)
* Zapp! (Optional)

Whether you're using **Android Studio** or **VSC**, take the time to learn the **shortcuts** and IDE plugins. Investing a few hours into this will pay off in the long run, saving you time and effort. It's worth learning the Flutter CLI as some tasks are faster to accomplish from the command line.

It's also important to develop a habit of using a version control system as early as possible. Git is currently the most popular option. While using the command line might seem cool, I recommend using a user-friendly Git client like **Fork**, **Sourcetree**, or one integrated into your **IDE**.

### Language

* Dart (Must have)
* OOP (Nice to have)
* Functional (Nice to have)
* Code Style (Optional)

It is important to follow code style, but if you’re entirely new, it might add frustration, so feel free to skip it for now but get back to it later. **“Effective Dart”** manual is a way to go. Use a strict linter like **very_good_analysis** from the beginning.

When it comes to OOP and Functional Programming, it's best to start with the basics. Don't worry about complex patterns or concepts like monads just yet. Focus on learning the fundamentals and building your skills gradually.

## Flutter

### Basic Widgets

* Material Widgets (Must have)
* Material Design (Must have)
* Cupertino Design (Nice to have)
* Mobile HIG (Optional)

Watch Widget of the Week on Youtube, explore material design concepts, get familiar with basic widgets Flutter shipping with.

Package of the Week show will introduce you to some of the most popular third-party widgets and packages available for Flutter.

### Core Design Patterns (Must have)

* Observer
* Command
* Dependency Injection
* State
* Composite
* Factory
* Builder
* Decorator

Design Patterns are the building blocks for developing robust applications. Understanding these patterns is essential for advanced development and gaining a deeper understanding of the framework itself. In addition, these patterns are universal and not specific to any particular framework or programming language. Therefore, investing time in studying them is a wise choice for future development work.

To start learning about design patterns, the old "Gang of Four" book is a great resource.

### Core Design Principles
  
* KISS (Must have)
* DRY (Must have)
* SOLID (Nice to have)

KISS and DRY should be your tactical focus during software development, but it's also essential to build on a solid foundation of strategic principles like SOLID. The book 'Clean Code' by Uncle Bob is a valuable resource that will help you in all of these areas.

I suggest using **Provider** or **get_it** for dependency injection. If you're feeling adventurous and want to try code generation, the **injectable** package is an excellent option.

### Networking
  * RESTful API (Must have)
  * JSON (Must have)
  * TCP/IP Sockets (Optional)
  * GraphQL (Optional)

It's important to understand how networking works and the magic behind front-end and back-end communication.Use code generation in production. 

**Retrofit**, **dio**, and **json_serializable** are your best friends here.

You’re interested in GraphQL - go for **ferry**.

### Simple Persistence**
  
* Serializers (Must have)
* Local storage (Must have)
* Keychain (Optional)
* Keystore (Optional)

Storing data is a common requirement for almost every app, but not every app needs a large storage solution. In many cases, it's best to keep things simple and use basic persistence when it's sufficient. The **shared_preferences** plugin, or its alternatives, can be a good option to consider for this purpose.


## Getting Deeper
### Database

* Isar (Must have)
* SQLite (Optional)
* Firebase (Must have)
* iCloud (Optional)

When you need to scale up your data storage, it may be time to consider more mature solutions, or even cloud-based options.

### Architecture** (Must have)

  * Redux
  * MVC
  * Lifting State
  * MVVM

It is fine to develop apps with Provider as long as you follow some architectural agreements or patterns. You may want to switch to **flutter_bloc**, **flutter_mobx**, **async_redux**, or other more architecture-aware patterns.

### Testing

* TDD (Must have)
* BDD (Nice to have)

When it comes to writing apps quickly, the key is to write them right the first time. To do this, start with the **TDD** approach and then transition to **BDD**. Kent Beck's book, **'Test-Driven Development by Example,'** is a great resource to get started with TDD. Additionally, Uncle Bob's **'Clean Code'** series covers the topic in depth

### Languages (Optional)
* Swift
* Kotlin
* FFIgen
* JNIgen

Learning native mobile development can help you gain a deeper understanding of the underlying platform, which can be valuable in fixing issues with third-party libraries or developing your own plugins. To get started, take the **Udacity course for Android** and the **Stanford Course for iOS**.

FFIgen and JNIgen will help us with access to your native code.

### Advanced Dart (Must have)

* Concurrent
* Reactive
* Functional

Now it is time to understand how async/await really works and why stateless is beneficial. Using packages like **freezed** can help improve model management, while **fpdart** or **dartz** can help make your code more elegant. For a deeper understanding, I recommend taking a basic course on Closure or F#.

### Package Manager

* Pub (Must have)
* Popular Plugins (Must have)
* Maven (Optional)
* CocoaPods (Optional)

Create your own plugin. Feeling confident? Challenge yourself by creating a plugin with a native view. And if that's not enough, make sure to thoroughly test your plugin and ensure that it doesn't leak memory.

### Profiling

* Leaks (Must have)
* Allocations (Nice to have)
* Performance (Nice to have)
* Widgets (Nice to have)

  Understand how to find memory leaks and spot performance issues. Start with a talk by **Filip Hráček** on Flutter Europe on Youtube.
  
### Flutter Internals

* Framework Architecture (Nice to have)
* Dart VM (Optional)
* RenderObjects (Optional)
* Layouts (Optional)

To gain a deeper understanding of the framework, take the time to learn about Flutter's rendering pipeline and how it lays out your widgets. Check out resources like **'Flutter's Rendering Pipeline'** by Adam Barth and **'Flutter's Architecture'** by Ian Hickson to get started.

### Flutter Internals

* OWASP MASVS (Nice to have)
* freeRASP (Optional)

Imagine how you would feel if you discovered that someone had stolen your app and published it under a different name. **MASVS** will make you think about this and many other scenarios. **freeRASP** is the simplest (but not sufficient) way to protect your app from various security threats.

### Beyound Mobile

* Desktop & Web (Optiona)
* Server (Nice to have)

By leveraging the power of Flutter, you can create applications that are not constrained by the limitations of smartphones - don’t forget to explore Desktop and Web. 

If you're interested in full-stack development, frameworks like **dart_frog** may be worth checking out.

## Almost there

### Continuous Integration

* CI server (Must have)
* Test Builds Distribution (Must have)
* FastLane (Must have)
* Code metrics (Optional)

Avoid building production builds from your local development folder. Instead, consider using tools like Codemagic, Travis, GitHub Actions, Circle CI, or registering your development machine as a CI node for GitLab CI. Building a software development lifecycle and collecting code coverage and other metrics will help you maintain code quality. Check out **Danger**, **SonarQube**, and most importantly, **FastLane**. A strict linter is a must here.


### Analytics

* User Behavior Analytics (Must have)
* Crash Logging (Must have)
* A/B Testing (Optional)

Analytics are essential for understanding how users interact with your app and for making data-driven decisions. Firebase Analytics, Firebase Crashlytics, and DataDog are just a few of many services that offer analytics features for free.


### Store (Must have)

* AppStore Guidelines
* Google Play Guidelines
* App Store Connect
* Google Dev Console

You have a responsibility to advise your clients on what is possible and what is not in terms of legal compliance. This includes complying with privacy laws such as GDPR and CCPA, as well as adhering to the app store's policies and guidelines.

## The End

Refer to [flutter_roadmap](https://github.com/olexale/flutter_roadmap) for the latest version and links.
