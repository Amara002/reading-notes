# Cognito
***The Amplify Auth category provides an interface for authenticating a user. Behind the scenes, it provides the necessary authorization to the other Amplify categories. It comes with default, built-in support for Amazon Cognito User Pool and Identity Pool. The Amplify CLI helps you to create and configure the auth category with an authentication provider.***

## Configure Auth Category

- ***To start provisioning auth resources in the backend, go to your project directory and execute the command:***<br>
`amplify add auth`<br>

- ***To push your changes to the cloud, execute the command:***<br>
`amplify push`<br>

## Install Amplify Libraries

***Add the following dependency to your app's build.gradle along with others you added above in Prerequisites and click "Sync Now" when prompted:***<br>

`dependencies {`<br>
  `  implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'` <br>
`}`<br>

