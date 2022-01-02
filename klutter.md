---  
layout: post  
title: Write once, run anywhere: Klutter = Flutter + Kotlin Multiplatform
---  

Having worked with Flutter I can say I really like it. Dart was a breeze to learn coming from Java. Hot reload is the best thing since sliced bread, writing a native looking and feeling UI for iOS and Android once is a godsend and the speed with which you can churn out a MVP is ridiculous. While Flutter can be a bit too verbose to my liking, it still is a nice declarative way of building an UI.

Yet after a year I still decided to move to Kotlin Multiplatform. Why? There's a few reasons but only one was a real dealbreaker in the end: Dependency management. Once you start making something a bit more complex than a simple MVP, you probably want to start using native functionality. As an efficient (lazy?) developer you will first check if there are plugins available. Using one or two of them is fine, but keep adding more and at some point you will find yourself at a point where you can't upgrade a dependency to a newer version due to incompatible versions. It's a dependency nightmare. Well maybe not yet. But it will be when you find out some dependencies can actually just vanish in thin air because they are deprecated. Not really funny when you can't compile an app you haven't worked on for a few months because a dependency can't be pulled from pub anymore.

But of course that does not make Flutter bad.

### What can I do for you?
*


### Contact me

[info@buijs.dev](mailto:info@buijs.dev)