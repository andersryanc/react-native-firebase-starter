![Screen Recording](./sample.gif)

# React Native Firebase Starter

This project was created with `react-native init`. I then converted it to using cocoapods and installed [React Native Firebase v2](https://invertase.io/react-native-firebase/#/v2/) with `yarn add react-native-firebase`.

If you are downloading this project for the first time, be sure to setup your [iOS](https://invertase.io/react-native-firebase/#/v2/installation-ios) and [Android](https://invertase.io/react-native-firebase/#/v2/installation-android) google api keys (after setting up your firebase account / project) by following step 1 in each link. Both files should already be linked up in the projects - they just are not tracked by git.

- For iOS, copy in your `GoogleService-Info.plist` to the `ios` directory.
- For Android, copy in your `google-services.json` to the `android` directory.

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
