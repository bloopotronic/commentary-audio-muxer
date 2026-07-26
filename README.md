commentary-merge is a Perl utility for merging standalone movie commentary tracks with existing video files while preserving the original video stream. It uses ffprobe, ffmpeg, and SoX to analyze the source media, choose the right audio-processing path, and create output supporting mono, stereo, and 5.1 surround audio. Configuration files make it possible to adjust the audio mix and repeat the same processing later.

Some parts are more elaborate than they really need to be, especially the child-process management. That was partly intentional, since the project gave me a chance to build experience with Unix process control, interprocess communication, and signal handling.

The script also changed quite a bit over time, so some of the code reflects that. It would benefit from further cleanup, particularly splitting the larger pieces into separate modules.
