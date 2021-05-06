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

## Memory and Storage Usage Optimaization
Device storage is an important aspect of any app. As we work with media we keep using the disk space ofthe device. The private storage is being cleared in appropriate time and other things are left for the user to clear. Here comes the privacy. The media is their intellectual property which should be cleared by them.

## Camera and Library

