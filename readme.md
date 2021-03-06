![Screen Recording](./sample.gif)

# React Native Firebase Starter

This project was created with `react-native init`. I then converted it to using cocoapods and installed [React Native Firebase v2](https://invertase.io/react-native-firebase/#/v2/) with `yarn add react-native-firebase`.

# First Time Project Setup

Install project dependencies:

```bash
yarn
cd ios
pod install
```

For android, make sure you either open up android studio to have it generate a `android/local.properties` file or that you have your `ANDROID_HOME` environment variable set to the location of your android sdks.

Next, be sure to setup your [iOS](https://invertase.io/react-native-firebase/#/v2/installation-ios) and [Android](https://invertase.io/react-native-firebase/#/v2/installation-android) google api keys (after setting up your firebase account / project) by following step 1 in each link. Both files should already be linked up in the projects - they just are not tracked by git.

- For iOS, copy in your `GoogleService-Info.plist` to the `ios` directory.
- For Android, copy in your `google-services.json` to the `android/app` directory.

# Firebase database setup

This super simple example app expects you to have a root node in your database with a child of `names` which has a set of child nodes with random names for each value, like:

```
example-app -
  names -
    0 - joe
    1 - jane
    2 - john
    3 - ...
```
