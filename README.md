# VideoColorMatch
Match the color grading and noise/grain between two video clips.  Automatically adjusts brightness, contrast, tint/temperature, saturation, highlights, shadows, noise/grain, etc to match a reference video.

Download link: https://github.com/pftq/VideoColorMatch/releases/tag/20261105<br>
You may also find these useful (one-click to download all [here](https://drive.google.com/drive/folders/1nvQFC5uwsZlf-82LuskCP-qut9xHw-lt?usp=sharing)):\
• [Video Debanding](https://github.com/pftq/Video-Debanding) (fixes quality issues with repeat re-processing/compression)\
• [Video Compare](https://github.com/pftq/Video-Compare) (to check export errors, differences, etc)\
• [MP4 Audio Delay Fix](https://github.com/pftq/MP4-Audio-Delay-Fix) (20ms delay at start of file)\
• [Video Frame Sync](https://github.com/pftq/Video-Frame-Sync) (syncing 2 files that drift out of sync)\
• [Video Splicer](https://github.com/pftq/Video-Splicer) (trim or join MP4s without re-encoding)\
• [Screencaps Generator](https://github.com/pftq/Screencaps-Generator) (smart screencaps selection + gallery grid sheet)\
• [Video To Selective Color](https://github.com/pftq/Video-To-Selective-Color) (selectively leave things in color on black-and-white video)

This is a tool I built for myself for similar shots or edit passes on the same footage having ever so slight color drift. This has happened with me for Adobe exports that apply an ever so slight tint to MP4s which accumulate on multiple passes. 

This is also useful for AI video editing that often slightly changes the color.  For WAN VACE, it also ignores the masked areas/frames, so you can just drag the same input video in used for VACE.  If you are using Seedance, Seedance tends to also cause frames to drift out of sync, so you may want to check out Video-Frame-Sync https://github.com/pftq/Video-Frame-Sync instead (which includes the same color match algo as this repo).

Lastly, as a bonus, I also included a rudimentary noise/grain match.  You can also drop a single frame as input to match color/sizing to.

Update 2026/11/17: 
- This is now functionally the same app as VideoFrameSync but with different defaults catered to color correcting, but if you have VideoFrameSync it already can do everything this app does (and vice versa) https://github.com/pftq/Video-Frame-Sync
- I also gave an option to ignore if the reference and edit clips are not close matches for color matching, so this can now be used to match color grading/noise to a completely different scene.

<img width="873" height="648" alt="image" src="https://github.com/user-attachments/assets/938a3b70-200d-4506-bb80-4bdbe7108c68" />

Credits:
- Python, application runtime
- Tcl/Tk, user interface
- NumPy, numerical processing
- OpenCV, image processing
- Pillow, image previews
- PyAV / FFmpeg, video and audio decoding/encoding
- PyInstaller, Windows executable packaging
