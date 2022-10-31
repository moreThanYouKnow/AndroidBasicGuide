# Android Basics Guide
Guide to all basic Android Dev tricks in one file! This repository is open to your suggestions and pull requests. It contains many links on various important Android Development topics. What's important in Android Development? Just add your own links and text recommendations!

## Architecture as it is

If you're looking for something official, you can watch some good explanations here:  
Official guide to app architecture: https://developer.android.com/topic/architecture
Good course from Google: https://developer.android.com/courses/pathways/android-architecture

But we also want to share this beautiful author's articles with you. Don't be afraid to read them:

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

Official (and so qualitative!) materials on retrofit basics: https://futurestud.io/learningpaths/retrofit-basics

Unofficial (but also very good) article: https://medium.com/@prakash_pun/retrofit-a-simple-android-tutorial-48437e4e5a23

How to trust all HTTPS certificates: https://futurestud.io/tutorials/retrofit-2-how-to-trust-unsafe-ssl-certificates-self-signed-expired
(We don't recommend you do that! :))

## In-App Billing

In-App Billing mechanisms, unfortunately, change every year. But here you can get the most relevant info on billing integration:
https://developer.android.com/google/play/billing/integrate

Official Google Billing guide: https://developer.android.com/google/play/billing/billing_library_overview

Old explanation on Habr: https://m.habr.com/ru/post/444072/

Serso Billing library: https://github.com/serso/android-checkout

Really important links (with some samples like TrivialDrive!):

https://developer.android.com/google/play/billing/integrate?authuser=0&skip_cache=true#pending

https://accounts.google.com/o/oauth2/v2/auth?client_id=721724668570-nbkv1cfusk7kk4eni4pjvepaus73b13t.apps.googleusercontent.com&redirect_uri=https%3A%2F%2Fdeveloper.android.com%2Foauth2callback&scope=openid+https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fuserinfo.email+https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fdeveloperprofiles+https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fdeveloperprofiles.award+https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fuserinfo.profile+https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fgoogledevelopers&access_type=online&response_type=code&state=%7B%22csrf_token%22%3A+%229fbc30ffaab96b502a3a751a1238638ec7d79e9b6403ed7d30fea677802fe2b8%22%2C+%22return_url%22%3A+%22https%3A%2F%2Fdeveloper.android.com%2Fgoogle%2Fplay%2Fbilling%2Fintegrate%3Fauthuser%3D0%26skip_cache%3Dtrue%22%7D&prompt=none&auto_signin=True#pending

https://stackoverflow.com/questions/62504562/google-play-billing-api-how-to-understand-the-user-is-subscribed

https://github.com/android/play-billing-samples/blob/main/TrivialDriveKotlin/app/src/main/java/com/sample/android/trivialdrivesample/TrivialDriveApplication.kt

https://github.com/android/play-billing-samples/blob/main/TrivialDriveKotlin/app/src/main/java/com/sample/android/trivialdrivesample/billing/BillingDataSource.kt

https://stackoverflow.com/questions/47990462/using-live-data-how-to-display-a-dialog-only-once

https://github.com/android/play-billing-samples/blob/main/ClassyTaxiJava/app/src/main/java/com/sample/android/classytaxijava/billing/BillingClientLifecycle.java

https://stackoverflow.com/questions/66010079/google-play-billing-library-3-0-restore-purchase

## Local Data: SQLite + Room

5 steps to implement Room persistance library: https://android.jlelse.eu/5-steps-to-implement-room-persistence-library-in-android-47b10cd47b24

Room StartAndroid lessons: https://startandroid.ru/ru/courses/architecture-components/27-course/architecture-components/532-urok-8-room-query.html

SQLite debug: https://medium.com/better-programming/android-best-sqlite-debugging-tools-a9a8da07568f

Do I need to call suspend functions of Retrofit and Room on a background thread? https://proandroiddev.com/do-i-need-to-call-suspend-functions-of-retrofit-and-room-on-a-background-thread-26650dac762d

## Permission requests

Permissions on Android: https://developer.android.com/guide/topics/permissions/overview

Request app permissions: https://developer.android.com/training/permissions/requesting
(official explanation)

Permissions and Material Design: https://material.io/design/platform-guidance/android-permissions.html

## UI: RecyclerViews are important!

Example of usage DiffUtil with RecyclerView: https://github.com/guenodz/livedata-recyclerview-sample/blob/master/app/src/main/java/me/guendouz/livedata_recyclerview/PostsAdapter.java

Use case: DragSelect RecyclerView like Google Photos: https://github.com/afollestad/drag-select-recyclerview

ViewPager and it's pages with RecyclerView: How to Fix ViewPager scrolling issue? You can use this

    recyclerView.setNestedScrollingEnabled(false);
    
DiffUtils under the hood: https://www.youtube.com/watch?v=uhtYuvubVm8&feature=youtu.be

MergeAdapter. how to show data from different adapters in a one RecyclerView consequently? https://medium.com/@prafullmishra09/fuse-your-lists-with-mergeadapter-aedfa4af209b

RecyclerView and Touch Events: https://veldan1202.medium.com/touch-event-management-c69d156fda96

## UI: Custom Views and useful view libraries!

Using compound ViewGroups instead of many views: https://android.jlelse.eu/app-rating-bar-making-a-compound-viewgroup-in-android-adb2bd25f4cc

SubsamplingScaleImageView for your gallery image viewer: https://github.com/davemorrissey/subsampling-scale-image-view/

Increasing optimization: Lazy inflating fragment with ViewStub! https://medium.com/@raymondctc/android-performance-lazy-inflating-fragment-with-viewstub-b51b2682ec0c

Jetpack Compose equivalents! https://www.jetpackcompose.app/What-is-the-equivalent-of-TextView-in-Jetpack-Compose

Touch Event management: https://veldan1202.medium.com/touch-event-management-c69d156fda96

## UI: Widgets!
Create a simple widget (official tutorial by Google): https://developer.android.com/develop/ui/views/appwidgets

Create an advanced widget (official tutorial by Google): https://developer.android.google.cn/develop/ui/views/appwidgets/advanced

Complete explanation on widgets in Android (Medium article): https://medium.com/android-bits/android-widgets-ad3d166458d3

StartAndroid about widgets: https://startandroid.ru/ru/uroki/vse-uroki-spiskom/195-urok-117-vidzhety-sozdanie-lifecycle.html

## Dependency Injection: Dagger alternatives!

Koin vs Dagger, Say hello to Koin: https://link.medium.com/Vfu6MrGjnU

Koin's official website: https://insert-koin.io/

Koin: Lightweight Dependency Injection Framework: https://www.baeldung.com/kotlin/koin-di



## Building faster, building better

Shrinking apk size and build time: https://medium.com/linedevth/build-your-android-app-faster-and-smaller-than-ever-25f53fdd3cdc

Decreasing app size using modules: https://playacademy.exceedlms.com/student/path/13019-decrease-app-size-and-deliver-features-on-demand?utm_source=newsletter&utm_medium=email&utm_campaign=AAB_newsletter

Dealing with invisible Gradle dependencies: https://proandroiddev.com/android-gradle-and-the-curious-case-of-invisible-dependency-7f1bcc8bb79e

Incremental annotation processing for faster builds: https://habr.com/ru/company/hh/blog/484918/

Speeding up Android Studio:
https://medium.com/@ankushkapoor2015/how-to-speed-up-android-studio-43aed38d248f

Gradle Experimental feature to increase building speed: https://blog.gradle.org/introducing-file-system-watching

Build speed optimization: https://www.crazylegend.dev/2020/07/optimize-build-speeds-for-your-android.html
