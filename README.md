# Android Basics Guide
Guide to all basic Android Dev tricks in one file! This repository is open to your suggestions and pull requests. It contains many links on various important Android Development topics. Just add your own!

## Architecture as it is

Why should your app be Single Activity with fragments: https://m.habr.com/ru/company/redmadrobot/blog/426617/

Android Architecture Components: Room, LiveData -> ViewModel: https://medium.com/@gadi.krn/android-architecture-components-make-your-app-as-you-dreamed-9a786fce67ea

Typical mistakes with Architecture Components: https://devcolibri.com/5-common-mistakes-when-using-architecture-components/

Sample of clean and modularized Android app: https://proandroiddev.com/android-architecture-d7405db1361c

When to load data in ViewModels? https://proandroiddev.com/when-to-load-data-in-viewmodels-ad9616940da7

Multi-modules & MVVM (Google Clean Architecture): https://proandroiddev.com/android-architecture-d7405db1361c

Note: ViewModel doesn't replace onSaveInstanceState! onSaveInstanceState is used for local UI state (not reliable on data). ViewModel destroying when app goes to background for a long time but onSaveInstanceState data remains, and you can obtain it in onCreate or some other methods.

Internals of Android OC: Stack Architecture: https://proglib.io/w/4970e537

## Long asynchronous operations: Coroutines

Basic coroutines recipes: https://proandroiddev.com/android-coroutine-recipes-33467a4302e9

Google CodeLabs lesson: https://codelabs.developers.google.com/codelabs/kotlin-coroutines/


Threads/Coroutines for beginners (with architecture): https://android.jlelse.eu/android-threads-coroutines-for-beginners-f39abc90d927

Coroutines with Clean Architecture: https://proandroiddev.com/android-architecture-d7405db1361c


Patterns/antipatterns: https://proandroiddev.com/kotlin-coroutines-patterns-anti-patterns-f9d12984c68e

Popular mistakes: https://medium.com/google-developer-experts/misnomers-mistakes-and-misunderstandings-to-watch-for-when-learning-kotlin-coroutines-and-flow-2744186be3e

## Internet API Requests: Retrofit

How to trust all HTTPS certificates: https://futurestud.io/tutorials/retrofit-2-how-to-trust-unsafe-ssl-certificates-self-signed-expired

## Local Data: SQLite + Room

5 steps to implement Room persistance library: https://android.jlelse.eu/5-steps-to-implement-room-persistence-library-in-android-47b10cd47b24

Room StartAndroid lessons: https://startandroid.ru/ru/courses/architecture-components/27-course/architecture-components/532-urok-8-room-query.html

SQLite debug: https://medium.com/better-programming/android-best-sqlite-debugging-tools-a9a8da07568f

Do I need to call suspend functions of Retrofit and Room on a background thread? https://proandroiddev.com/do-i-need-to-call-suspend-functions-of-retrofit-and-room-on-a-background-thread-26650dac762d

## Building faster, building better

Shrinking apk size and build time: https://medium.com/linedevth/build-your-android-app-faster-and-smaller-than-ever-25f53fdd3cdc

Decreasing app size using modules: https://playacademy.exceedlms.com/student/path/13019-decrease-app-size-and-deliver-features-on-demand?utm_source=newsletter&utm_medium=email&utm_campaign=AAB_newsletter

Dealing with invisible Gradle dependencies: https://proandroiddev.com/android-gradle-and-the-curious-case-of-invisible-dependency-7f1bcc8bb79e

Better dependency management with Android Studio 3.5+ : prglb.ru/24r6s

Incremental annotation processing for faster builds: https://habr.com/ru/company/hh/blog/484918/

Speeding up Android Studio:
https://medium.com/@ankushkapoor2015/how-to-speed-up-android-studio-43aed38d248f

Gradle Experimental feature to increase building speed: https://blog.gradle.org/introducing-file-system-watching

Build speed optimization: https://www.crazylegend.dev/2020/07/optimize-build-speeds-for-your-android.html
