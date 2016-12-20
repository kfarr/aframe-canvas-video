# aframe-canvas-video
A hacky experiment to play video in DOM canvas element and then render canvas as a texture in A-Frame VR.

This works, kind of. It's not the "right" way to do this as it duplicates the rendering of video to the canvas object which is not really optimized for this sort of use case. Further, it will likely break down at larger resolutions that would be desirable for 360 video, so its use is limited.

The canvas video player code is from the git project [html-canvas-video-player](https://github.com/Stanko/html-canvas-video-player), originally created as a workaround for autoplaying videos inline on iOS. Recently Apple announced support for inline playback so this workaround is no longer needed, but using the canvas for video playback gives us some interesting ways to experiment putting video or other graphics into VR.

Other resources:
* [aframe-video-shader](https://github.com/mayognaise/aframe-video-shader) is a more feature rich implementation using canvas for video playback inside of aframe.
