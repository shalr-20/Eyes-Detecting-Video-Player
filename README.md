# Eyes Detecting Video Player
The application will utilize eye detection technology using third party library to enhance the user experience by ensuring that video content plays only when the user's eyes are detected. This feature is designed to improve engagement, conserve resources, and maintain privacy by pausing the video automatically when eye presence is not detected and resuming playback once the user’s eyes are back in view. This technology can be particularly useful in media streaming apps, educational tools, or situations where user attention is critical, providing a seamless, efficient, and user-friendly experience.

## Key functionality:

- **Eye detection:** Uses the device's front camera to continuously detect the presence of the user's eyes.
  
- **Automated video control:** The app will pause the video when no eyes are detected, and resume when eyes are present, ensuring that the content is only played when the user is actively watching.
  
- **Privacy-focused:** No personal data is stored; eye detection is performed in real-time and is used solely for controlling video playback.

## Usage:

1) To add mode to be fast or accurate and cameraFace to be front or back:
```gradle
public void init(Context activityContext, String mode, String cameraFace){}
```

2) To add mode to be accurate or fast:
```gradle
public void init(Context activityContext, String mode){}
```

3) To access if the user smiled during the video:
   - For this, just use this initWithSmilingStatus() method instead of the normal init() like this:
```gradle
lookAtMe.initWithSmilingStatus(this)
```

## Prerequisites (For latest Android Studio version)
Add this in your settings.gradle.kts (Project Settings):
```gradle
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        maven { url = uri("https://www.jitpack.io") }
    }
}
```

## Dependency
1) Add this to your module's build.gradle file (make sure the version matches the JitPack badge above):
```gradle
dependencies {
	        implementation ("com.github.Pradyuman7:LookAtMe:Version1.0")
}
```

2) For latest release, please check the JitPack version and match it with the dependency.
```gradle
dependencies {
	        implementation ("com.github.Pradyuman7:LookAtMe:Version2.0")
}
```

## Pull Request
If you have new ideas or discover a bug, feel free to open an issue or submit a pull request.

## Credits

Third party library is taken from [LookAtMe](https://github.com/Pradyuman7/LookAtMe/tree/master?tab=readme-ov-file)
