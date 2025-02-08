# Expo Android Build Failure: Unclear Dependency Errors

This repository demonstrates a bug in the Expo CLI where Android builds fail with confusing dependency-related errors, while iOS builds succeed.  The problem stems from a combination of factors, including the complexity of Expo's build system and its interactions with React Native's native module system. The exact error messages can vary but often involve missing native libraries or incorrect configurations within the build process.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Attempt to build an Android APK using `expo build:android`.  Note the error messages.
4. Compare this behavior to building an iOS IPA using `expo build:ios`, which should complete successfully.

## Potential Causes

* Inconsistent package versions across dependencies.
* Conflicts between Expo modules and third-party libraries.
* Issues with Android build tools or SDK configurations.
* Incorrectly configured native modules within the project.

## Solution

The provided `bugSolution.js` offers a potential workaround.  There may be other solutions depending on the specific error messages encountered.