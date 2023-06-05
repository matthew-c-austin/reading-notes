# Read: Class 34

## Reflections

This reading assignment covers Google's guide to app publishing. It explores key concepts of versioning and release preparation for Android applications, along with the steps necessary to successfully publish an application on the Google Play Store.

## Readings

[Google’s app publishing guide](https://developer.android.com/studio/publish)

1. How are releases and versioning related?

    Releases and versioning are closely related as each release of an application should have a unique version number. The versioning helps in keeping track of different updates or modifications in the application. It is important for handling updates, troubleshooting issues, and for users to distinguish between different versions of the app.

2. What are the 5 main tasks you need to complete to prepare your application for release to the Google Play Store?

    1. Configuring the app’s build.gradle file for release: This includes setting the applicationId, versionCode, and versionName.
    2. Building an unsigned APK: This is essentially the package file that includes all your app's code and resources.
    3. Signing the APK: All applications on the Play Store need to be digitally signed with a private key before they can be installed or updated on a user's device.
    4. Testing the signed APK: This ensures the APK works as expected and doesn't have any major issues.
    5. Distributing the APK: Once tested, the APK can be distributed either directly through Google Play Store or through other channels.

## Things I want to know more about

1. I am interested in understanding more about the differences in preparing an app for Google Play Store vs. Apple's App Store. What are the key differences between the two in terms of versioning, signing, and distribution process?
