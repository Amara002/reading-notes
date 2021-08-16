# Espresso
***Espresso is targeted at developers, who believe that automated testing is an integral part of the development lifecycle. While it can be used for black-box testing, Espresso’s full power is unlocked by those who are familiar with the codebase under test.***

# Record an Espresso test
***Espresso tests consist of two primary components: UI interactions and assertions on View elements. UI interactions include tap and type actions that a person may use to interact with your app. Assertions verify the existence or contents of visual elements on the screen. For example, an Espresso test for the Notes testing app might include UI interactions for clicking on a button and writing a new note but would use assertions to verify the existence of the button and the contents of the note.***

***This section will go over how to create both of these test components using Espresso Test Recorder, as well as how to save your finished recording to generate the test.***

# Record UI interactions

***To start recording a test with Espresso Test Recorder, proceed as follows:***

1. ***Click Run > Record Espresso Test.***
2. ***In the Select Deployment Target window, choose the device on which you want to record the test. If necessary, create a new Android Virtual Device. Click OK.***
3. ***Espresso Test Recorder triggers a build of your project, and the app must install and launch before Espresso Test Recorder allows you to interact with it. The Record Your Test window appears after the app launches, and since you have not interacted with the device yet, the main panel reads "No events recorded yet." Interact with your device to start logging events such as "tap" and "type" actions.***

 # Add assertions to verify UI elements

***Assertions verify the existence or contents of a View element through three main types:***

- ***text is: Checks the text content of the selected View element***
- ***exists: Checks that the View element is present in the current View hierarchy visible on the screen***
- ***does not exist: Checks that the View element is not present in the current View hierarchy***