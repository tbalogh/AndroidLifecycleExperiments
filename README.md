# AndroidLifecycleExperiments

Android Architecture Components introduce (https://developer.android.com/topic/libraries/architecture/lifecycle)[Lifecycle-aware components] 
that helps to live in peace and harmony with UI components whose lifecycle managed by the Android OS, such as Activities and Fragments.

We are commonly interested in these (https://developer.android.com/reference/android/arch/lifecycle/Lifecycle.Event)[Lifecycle events] 
so we can avoid common gotchas of the Activities and Fragments, such as updating them while our application is in the background.   

The Activities and Fragments are implements the (https://developer.android.com/reference/android/arch/lifecycle/LifecycleOwner)[LifecycleOwner] interface 
so we can easily observe those lifecycle events.

There are already built-in components, such as (https://developer.android.com/topic/libraries/architecture/livedata)[LiveData] 
that exploit the benefits of these Lifecycle concept.

However we have interests in these lifecycle events in some cases, such as logging or reporting.

These repository is a simple case where I implement a lifecycle logger using these new components.   
