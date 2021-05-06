<div align="center">
  <a href="https://apps.apple.com/in/app/brbck/id1532417088"><img src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/56ec0af85d2fb486130322fee250c3f2062fd0af/brbck-header.png" alt="BRBCK Header"></a>
</div>
<p align="center">
  <img alt="Build Status" src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/56ec0af85d2fb486130322fee250c3f2062fd0af/B-Passing.png" height="30px">
  <img alt="Build Number" src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/dbd84fe56195e13a9d7ce2998fdf35bee364a9db/B-Number.png" height="30px">
  <img alt="Platform: iOS" src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/9c7cbd97bab0ef21df3e0f08adf610a2f5035d81/P-ios.png" height="30px">
  <img alt="Category: Social Media" src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/9c7cbd97bab0ef21df3e0f08adf610a2f5035d81/C-SM.png" height="30px">
</p>

# Change Log
**Version 8.0 build 1.1.16**

### Content
- [Hardware Usage Optimaization](#hardware-usage-optimization)
- [Memory and Storage Usage Optimaization](#memory-usage-optimization)
- [Camera and Library](#camera-and-library)

## Hardware Usage Optimaization
iOS is efficient with less *Application Memory (RAM)* which requires us to take care of the operations we create. Most of the heavy tasks are now being run in suitable **Threads**. The operations are being executed asynchronously and being closed properly so not to take up huge amount of unpermitted memory usage.
Operations like handling media and data have been moved to different processes decoupled from the main process of the app.

### Location
Location usage is limited for only when needed.

### External devices
Video and sound can be played in external devices. Available in location based post filter scenes.

## Memory and Storage Usage Optimaization
Device storage is an important aspect of any app. As we work with media we keep using the disk space of the device. The private storage is being cleared in appropriate time and other things are left for the user to clear. Here comes the privacy. The media is their intellectual property which should be cleared by them.

## Camera and Library
- The old method of using a third party library is ditched and new classes using system APIs for video and audio devices have been written from scratch.
- Camera now detects subject brightness and can use flash when needed.
- Camera now knows the system pressure level at which it operates. It can throttle frame rate indicating that there is serious or shut-down-level system pressure. The view finder of the camera would be smaller in these cases.
- App plays haptics and new sounds whenever necessary for better experience.
- App has adapted to Photos framework and its APIs for better and optimized experience while browsing media from library.
- App can download and use media from iCloud if the media is not available in phone's storage.
- **Multi Shot from camera:** Camera can now capture and store up to 5 media at once for editing and uploading.
- **Video range scrubbing:** For videos longer than 20 seconds, users will now be able to scrub through the video and select desired range


### Attachments and Misc.
- The new module provides and broader range of stickers, gifs, text styles and colors, doodling. 
- System information such as location and clock can now be used in attachments.

## Media in Feed
- Reusing the same videoPlayer for every video in feed eliminating the possibility of simultaneous video play.
- Configurations for video player and image donloader has been changed for faster loading of the media.
- Comments and Post details have been moved to separate new scenes.

## Chat
- Image and video operations are faster than before
- Uses the same flow for Camera and Library
- Now supports memoji
- Supports pasting image from external sources directly in message box.

### Notification Interaction
- Tapping on a notification will directly open the post.
