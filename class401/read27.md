# Intents, Activities, and SharedPreferences

## Managing Tasks

***You can do these things and more, with attributes in the `<activity>` manifest element and with flags in the intent that you pass to `startActivity()`.***

***In this regard, the principal `<activity>` attributes you can use are:***

- **taskAffinity**
- **launchMode**
- **allowTaskReparenting**
- **clearTaskOnLaunch**
- **alwaysRetainTaskState**
- **finishOnTaskLaunch**

***And the principal intent flags you can use are:***

- **FLAG_ACTIVITY_NEW_TASK**
- **FLAG_ACTIVITY_CLEAR_TOP**
- **FLAG_ACTIVITY_SINGLE_TOP**

***In the following sections, you'll see how you can use these manifest attributes and intent flags to define how activities are associated with tasks and how they behave in the back stack.***


## Save key-value data

***If you have a relatively small collection of key-values that you'd like to save, you should use the `SharedPreferences` APIs. A `SharedPreferences` object points to a file containing key-value pairs and provides simple methods to read and write them. Each `SharedPreferences` file is managed by the framework and can be private or shared.***

### Get a handle to shared preferences
***You can create a new shared preference file or access an existing one by calling one of these methods:***

- ***`getSharedPreferences()` — Use this if you need multiple shared preference files identified by name, which you specify with the first parameter. You can call this from any `Context` in your app.***

- ***`getPreferences()` — Use this from an `Activity` if you need to use only one shared preference file for the activity. Because this retrieves a default shared preference file that belongs to the activity, you don't need to supply a name.***
