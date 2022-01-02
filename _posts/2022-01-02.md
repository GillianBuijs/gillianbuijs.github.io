---  
layout: post  
title: Really write once: Klutter = Flutter + Kotlin Multiplatform
---  

Klutter is a framework and tool set which uses Flutter to create the frontend
and Kotlin Multiplatform for the backend. The connective layer is generated
by the Klutter framework. Klutter combines industry best practices
for everything from app design to CICD into a single cohesive framework.

And I made it.

## Why I made Klutter
Having worked with Flutter I can say I really like it. Dart was a breeze to learn coming from Java.
Hot reload is the best thing since sliced bread, writing a native looking and feeling UI for iOS and
Android once is a godsend and the speed with which you can churn out a MVP is ridiculous. While
Flutter can be a bit too verbose to my liking, it still is a nice declarative way of building an UI.

Yet after a year I still decided to move to Kotlin Multiplatform. Why? For starters I have to say
dependency management in Flutter/Dart is not very good. Once you start making something a bit more complex
than a simple MVP, you probably want to start using native functionality. As an efficient
(lazy?) developer you will first check if there are libraries available. Using one or two of them is fine,
but keep adding more and soon you will get caught in a dependency nightmare. If you are really unlucky
some libraries you need will just vanish in thin air because they are deprecated. In this regard
Kotlin Multiplatform is not all that much better, mostly because of the lack of available
libraries.

However that's much less of an issue in KMP than it is in Flutter. If you're focussed on
Flutter you will be using Dart as a programming language. When you want to use native functionality you
can either choose to use 3rd party libraries (which can be a bad choice as said above) or you can write
the native code yourselves. Doing that means writing code in Kotlin or Java for Android and in Objective-C
or Swift for iOS. So if you want to be in full control of your app and write as much as possible yourself
then you have no other option than to write in 3 different programming languages. When using KMP you can
use Kotlin for both Android and iOS native functionality, making it a lot more accessible.

These points are relevant for the backend code but looking at the frontend things are a little different.
In contrast to what is discussed above, Flutter is a lot more accessible for frontend development than
Kotlin Multiplatform. Both Flutter and KMP can create native (looking/feeling) UI. With Flutter
you will however only have to do this once. Using KMP you will have to create a UI with Kotlin for Android
and for iOS with Swift. Now Kotlin and Swift are very similiar programming languages so it won't be hard
for a Kotlin programmer to start using Swift. A very nice comparison can be read on
[https://www.raywenderlich.com](https://www.raywenderlich.com/6754-a-comparison-of-swift-and-kotlin-languages).

Kotlin and Swift might be very similiar, but it does not take away the fact you will have to write code
twice instead of once. I initially chose to work with Flutter because I did not want to write an UI twice
so was I really going to do this? I created a little MVP with KMP but I was not convinced this was the way.
I don't want to write an UI twice. I don't want to write backend code twice. I got Flutter... I got KMP. Why
not use both? And that's when Klutter was created. I did a POC manually hooking up a KMP library into a
Flutter app and after a few headaches it worked. At first I wanted to publish a template to create
a Flutter + KMP app from scratch. Since then it has evolved to a complete framework to not just only
make Flutter and KMP work together, but also add everything to publish an app to the Playstore/App Store.

Klutter is in a pre-alpha stage meaning it is just getting started and a lot can/will change before
it is production ready. Curious? Have a look at the source and documentation:
[Klutter]([https://github.com/buijs-dev/klutter]). The next articles will discuss how Klutter works
and what milestones are expected for the near future.