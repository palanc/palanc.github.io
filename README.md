Run 'jekyll serve' to launch website at http://localhost:4000

.gif creation: The folowing are instructions for creating .gifs. Given a (1280x720) 30FPS .mp4:
1. Use the following command to extract all image frames:
 ffmpeg -i <name>.mp4 ./<name>_frames%05d.png
2. (Optional) Delete every other frame:
 rm *1.png *3.png *5.png *7.png *9.png
3. In gimp, File -> Open as Layers, select all of the frames
4. (Optional) Reduce size of frames to 640x360 using Image -> Scale Image
5. Choose Filters -> Animation -> Optimize (for GIF)
6. Choose File -> Export As..., and in the lower left choose Select File Type -> GIF Image
7. Make sure As Animation and Loop Forever are enabled before exporting
