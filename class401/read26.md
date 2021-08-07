# Application Fundamentals

***The Android SDK tools compile your code along with any data and resource files into an APK or an Android App Bundle.***

- **An Android package, which is an archive file with an .apk suffix, contains the contents of an Android app that are required at runtime and it is the file that Android-powered devices use to install the app.**

- **An Android App Bundle, which is an archive file with an .aab suffix, contains the contents of an Android app project including some additional metadata that is not required at runtime.**

## App components
***There are four different types of app components:***
1. **Activities**<br>
***An activity facilitates the following key interactions between system and app:***
- **Keeping track of what the user currently cares about (what is on screen) to ensure that the system keeps running the process that is hosting the activity.**
- **Knowing that previously used processes contain things the user may return to (stopped activities), and thus more highly prioritize keeping those processes around.**
- **Helping the app handle having its process killed so the user can return to activities with their previous state restored.**
- **Providing a way for apps to implement user flows between each other, and for the system to coordinate these flows. (The most classic example here being share.)**

2. **Services**<br>
***two different types of started services that modify how the system handles them:***

- **Music playback is something the user is directly aware of, so the app tells the system this by saying it wants to be foreground with a notification to tell the user about it; in this case the system knows that it should try really hard to keep that service's process running, because the user will be unhappy if it goes away.**
- **A regular background service is not something the user is directly aware as running, so the system has more freedom in managing its process. It may allow it to be killed (and then restarting the service sometime later) if it needs RAM for things that are of more immediate concern to the user.**

3. **Broadcast receivers**<br>
***A broadcast receiver is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements. Because broadcast receivers are another well-defined entry into the app, the system can deliver broadcasts even to apps that aren't currently running.***

4. **Content providers**<br>
***There are a few particular things this allows the system to do in managing an app:***

- **Assigning a URI doesn't require that the app remain running, so URIs can persist after their owning apps have exited. The system only needs to make sure that an owning app is still running when it has to retrieve the app's data from the corresponding URI.**
- **These URIs also provide an important fine-grained security model. For example, an app can place the URI for an image it has on the clipboard, but leave its content provider locked up so that other apps cannot freely access it. When a second app attempts to access that URI on the clipboard, the system can allow that app to access the data via a temporary URI permission grant so that it is allowed to access the data only behind that URI, but nothing else in the second app.**

## Activating components

***Three of the four component types—activities, services, and broadcast receivers—are activated by an asynchronous message called an intent. Intents bind individual components to each other at runtime. You can think of them as the messengers that request an action from other components, whether the component belongs to your app or another.***

***An intent is created with an `Intent` object, which defines a message to activate either a specific component (explicit intent) or a specific type of component (implicit intent).***

***There are separate methods for activating each type of component:***

- **You can start an activity or give it something new to do by passing an `Intent` to `startActivity()` or `startActivityForResult()` (when you want the activity to return a result).**
- **With Android 5.0 (API level 21) and later, you can use the `JobScheduler` class to schedule actions. For earlier Android versions, you can start a service (or give new instructions to an ongoing service) by passing an `Intent` to `startService()`. You can bind to the service by passing an `Intent` to `bindService()`.**
- **You can initiate a broadcast by passing an `Intent` to methods such as `sendBroadcast()`, `sendOrderedBroadcast()`, or `sendStickyBroadcast()`.**
- **You can perform a query to a content provider by calling `query()` on a `ContentResolver`.**

## The manifest file
***Before the Android system can start an app component, the system must know that the component exists by reading the app's manifest file, `AndroidManifest.xml`. Your app must declare all its components in this file, which must be at the root of the app project directory.***

### Declaring components
***You must declare all app components using the following elements:***
- **`<activity>` elements for activities.**
- **`<service>` elements for services.**
- **`<receiver>` elements for broadcast receivers.**
- **`<provider>` elements for content providers.**

> ***Activities, services, and content providers that you include in your source but do not declare in the manifest are not visible to the system and, consequently, can never run. However, broadcast receivers can be either declared in the manifest or created dynamically in code as BroadcastReceiver objects and registered with the system by calling registerReceiver().***