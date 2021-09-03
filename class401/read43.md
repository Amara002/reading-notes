# Kinesis & Analytics

## Set up Analytics backend

***Run the following command in your project's root folder. The CLI will prompt configuration options for the Analytics category such as Amazon Pinpoint resource name and analytics event settings.***
- `amplify add analytics`

## Install Amplify Libraries

***Expand Gradle Scripts, open build.gradle (Module: app). You will already have configured Amplify by following the steps in the Project Setup walkthrough.***

***Add Analytics by adding these libraries into the dependencies block:***<br>
`dependencies {`<br>
    `// Add these lines in dependencies`<br>
   ` implementation 'com.amplifyframework:aws-analytics-pinpoint:1.24.0'`<br>
   ` implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'`<br>
`}`

