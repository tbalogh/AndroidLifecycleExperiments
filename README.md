# AndroidLifecycleExperiments

This repository is a simple implementation of a lifecycle logger using the new [Android Architecture Components](https://developer.android.com/topic/libraries/architecture).

Android Architecture Components introduce [Lifecycle-aware components](https://developer.android.com/topic/libraries/architecture/lifecycle)
that help us to live in peace and harmony with UI components whose lifecycle managed by the Android OS, such as Activities and Fragments.

Android applications are commonly interested in these [Lifecycle events](https://developer.android.com/reference/android/arch/lifecycle/Lifecycle.Event) 
so we can avoid common gotchas, such as updating the UI while the application is in the background.   

The Activities and Fragments are implements the [LifecycleOwner](https://developer.android.com/reference/android/arch/lifecycle/LifecycleOwner) interface 
so we can easily observe those lifecycle events.

There are already built-in components, such as [LiveData](https://developer.android.com/topic/libraries/architecture/livedata),
that exploit the benefits of these Lifecycle components.

However there are other use cases of listening these lifecycle events, such as logging or reporting.

## Usage

Filter to the "LoggerLifecycleObserver" word in Logcat and see how activity and fragment lifecycles are called. The application consist of an activity and two fragments in that you can navigate between.

   
