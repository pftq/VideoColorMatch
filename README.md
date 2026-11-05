# VideoColorMatch
Match the color grading and noise/grain between two video clips.  Automatically adjusts brightness, contrast, tint/temperature, saturation, highlights, shadows, noise/grain, etc to match a reference video.

Download link: [https://github.com/pftq/Video-Compare/releases/tag/20261102](https://github.com/pftq/VideoColorMatch/releases/tag/20261105)

You may also find these useful:
- Video Debanding (fixes quality issues with repeat re-processing/compression) https://github.com/pftq/Video-Debanding
- Video Compare (to check export errors, differences, etc) https://github.com/pftq/Video-Compare
- MP4 Audio Delay Fix (20ms delay at start of file) https://github.com/pftq/MP4-Audio-Delay-Fix
- Video Frame Sync (syncing 2 files that drift out of sync) https://github.com/pftq/Video-Frame-Sync

This is a tool I built for myself for similar shots or edit passes on the same footage having ever so slight color drift. This has happened with me for Adobe exports that apply an ever so slight tint to MP4s which accumulate on multiple passes. 

This is also useful for AI video editing that often slightly changes the color.  For WAN VACE, it also ignores the masked areas/frames, so you can just drag the same input video in used for VACE.  If you are using Seedance, Seedance tends to also cause frames to drift out of sync, so you may want to check out Video-Frame-Sync https://github.com/pftq/Video-Frame-Sync instead (which includes the same color match algo as this repo).

Lastly, as a bonus, I also included a rudimentary noise/grain match.

<img width="873" height="648" alt="image" src="https://github.com/user-attachments/assets/938a3b70-200d-4506-bb80-4bdbe7108c68" />
