# Firebase UPM

If you are tired of Firebase Unity SDK polluting your project with folders and folders it is time to do it Unity Package Manager style. It also included `.asmdef` file to be compatible with your `.asmdef` enabled project. The name to reference is `Google.Firebase`.

## How

Clone this wherever you like and use UPM's offline package reference. Put a line like this in your `manifest.json`

```
"com.google.firebase": "file:../../Firebase/Assets",
```

You must travel the folder relatively from the `manifest.json` file location.

### One problem

Everything almost works in UPM, but there is one thing Firebase team hardcoded the path. That is generating the resource file. It specifically looks for your `Assets/Firebase/Editor/pythonfile` and cannot be somewhere else. To fix this, after linking your UPM you have to manually make that folder with that file copied from UPM package.

```
Generation of the Firebase Android resource file google-services.xml from Assets/SceneFiles/-FirebaseSettings/GoogleService-Info.plist failed.
If you have not included a valid Firebase Android resources in your app it will fail to initialize.
`python "/Users/Sargon/Documents/Projects/MelCadence/Assets/../Assets/Firebase/Editor/generate_xml_from_google_services_json.py" -i "Assets/SceneFiles/-FirebaseSettings/GoogleService-Info.plist" -l --plist`.

/usr/bin/python: can't open file '/Users/Sargon/Documents/Projects/MelCadence/Assets/../Assets/Firebase/Editor/generate_xml_from_google_services_json.py': [Errno 2] No such file or directory
```

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
