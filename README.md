# Chroma Keying using OpenCV

## Videos to Images and vice-versa

`cv2.VideoCapture` is a class for video capturing from video files, image sequences or cameras. We set the frame rate to be 0.5 seconds, which would capture the frame every 0.5 secods. That is, 2 frames per second. The program saves the images as `image[num].jpg` in an images folder.

For combining images into a video we add path variables to the image folder and set the images in a list. We sort this list in order so that we have the image sequence right. Using a frame-rate, here, 0.5, we can output a video in `.avi` format. 

## Capturing images from a webcam

Using the `cv2.VideoCapture` class, we can access the webcam. We keep the video displayed constantly, hitting the `SPACE` key clicks a picture which is saved in the images folder, as `opencv_frame_[num].jpg`. Hitting the `ESC` key quits the window.

## Chroma Keying Videos

Having a green screen video and another which would act as a background, we use openCV to mask the green screen. This was challenging as the window quit with an error, but still gave the desired output. 