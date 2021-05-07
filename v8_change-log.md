<div align="center">
  <a href="https://apps.apple.com/in/app/brbck/id1532417088"><img src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/186eb73f18fe93ec7d8ca9fe45e5a1a1cd4dd108/PNG/brbck-header.png" alt="BRBCK Header"></a>
</div>
<p align="center">
  <img alt="Build Status" src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/186eb73f18fe93ec7d8ca9fe45e5a1a1cd4dd108/PNG/B-Passing.png" height="25px">
  <img alt="Build Number" src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/186eb73f18fe93ec7d8ca9fe45e5a1a1cd4dd108/PNG/B-Number-8.png" height="25px">
  <img alt="Platform: iOS" src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/186eb73f18fe93ec7d8ca9fe45e5a1a1cd4dd108/PNG/P-ios.png" height="25px">
  <img alt="Category: Social Media" src="https://github.com/SwiftFoxx/code-images-ext-usage/blob/186eb73f18fe93ec7d8ca9fe45e5a1a1cd4dd108/PNG/C-SN.png" height="25px">
</p>

# Change Log
**Version 8.0 build 1.1.16**

### Content
- [Hardware Usage Optimaization](#hardware-usage-optimization)
- [Memory and Storage Usage Optimaization](#memory-usage-optimization)
- [Camera and Library](#camera-and-library)
- [Attachments and Misc](#attachments-and-misc)
- [Media in Feed](#media-in-feed)
- [Chat](#chat)
- [Notification Interaction](#notification-interaction)

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


### Attachments and Misc
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

## Notification Interaction
- Tapping on a notification will directly open the post.
