# Cave Mapper Python Script for Ravendawn

This is a simple Python script that takes a 1920x1080 video input of a player moving inside a cave in the game Ravendawn and outputs an image representing the whole map the player explored in the video.

The Image Processing algorithm extracts key points on two images and perform feature matching to obtain the translational movement between these images. Using the calculated movement, it then performs an image stitching to join these two images. The final image is a composition of several frames overlaid together using the `max` operator to try to preserve the lighting conditions.

# Demo

## Input Video
https://user-images.githubusercontent.com/49814646/175343031-2b2793e9-ceb0-402e-b813-38a74beba924.mp4

## Output Image
![result](https://user-images.githubusercontent.com/49814646/175343047-5388afa7-a8ea-4ac8-95f2-0392f208d0be.png)
