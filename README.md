# Eyes Detecting Video Player
The application will utilize eye detection technology to enhance the user experience by ensuring that video content plays only when the user's eyes are detected. This feature is designed to improve engagement, conserve resources, and maintain privacy by pausing the video automatically when eye presence is not detected and resuming playback once the user’s eyes are back in view. This technology can be particularly useful in media streaming apps, educational tools, or situations where user attention is critical, providing a seamless, efficient, and user-friendly experience.

## Key functionality:

- **Eye detection:** Uses the device's front camera to continuously detect the presence of the user's eyes.
  
- **Automated video control:** The app will pause the video when no eyes are detected, and resume when eyes are present, ensuring that the content is only played when the user is actively watching.
  
- **Privacy-focused:** No personal data is stored; eye detection is performed in real-time and is used solely for controlling video playback.

## Usage:

1) To add mode to be fast or accurate and cameraFace to be front or back:
```
public void init(Context activityContext, String mode, String cameraFace){}
```

2) To add mode to be accurate or fast:
```
public void init(Context activityContext, String mode){}
```

3) To access if the user smiled during the video:
   - For this, just use this initWithSmilingStatus() method instead of the normal init() like this:
```
lookAtMe.initWithSmilingStatus(this)
```
