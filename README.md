# Firebase UPM

If you are tired of Firebase Unity SDK polluting your project with folders and folders it is time to do it Unity Package Manager style.

## How

Clone this wherever you like and use UPM's offline package reference. Put a line like this in your `manifest.json`

```
"com.google.firebase": "file:../../Firebase/Assets",
```

You must travel the folder relatively from the `manifest.json` file location.

## What's included

- ✅ FirebaseAnalytics.unitypackage
- ✅ FirebaseAuth.unitypackage
- ✅ FirebaseDatabase.unitypackage
- ✅ FirebaseDynamicLinks.unitypackage
- ✅ FirebaseFunctions.unitypackage
- ✅ FirebaseInstanceId.unitypackage
- FirebaseInvites.unitypackage
- FirebaseMessaging.unitypackage
- ✅ FirebaseRemoteConfig.unitypackage
- ✅ FirebaseStorage.unitypackage

Why not that two? Because I am not using it in my game...

## Version

Version 5.2.0 - July 23, 2018
https://firebase.google.com/support/release-notes/unity
