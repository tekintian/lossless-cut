# Just for demo and DEV

 <p><b>LosslessCut</b></p>
  The swiss army knife of lossless video/audio editing
	<br>



LosslessCut aims to be the ultimate cross platform FFmpeg GUI for extremely fast and lossless operations on video, audio, subtitle and other related media files.
The main feature is lossless trimming and cutting of video and audio files, which is great for saving space by rough-cutting your large video files taken from a video camera, GoPro, drone, etc. It lets you quickly extract the good parts from your videos and discard many gigabytes of data without doing a slow re-encode and thereby losing quality. Or you can add a music or subtitle track to your video without needing to encode. Everything is extremely fast because it does an almost direct data copy, fueled by the awesome FFmpeg which does all the grunt work.

## Features

- Lossless cutting of most video and audio formats
- [Smart cut](https://github.com/tekintian/lossless-cut/issues/126) (experimental)
- Losslessly cut out parts of video/audio (for cutting away commercials etc.)
- Losslessly rearrange the order of video/audio segments
- Lossless merge/concatenation of arbitrary files (with identical codecs parameters, e.g. from the same camera)
- Lossless stream editing
  - Combine arbitrary tracks from multiple files (ex. add music or subtitle track to a video file)
  - Remove unneeded tracks
  - Replace or re-encode only some tracks
  - Extract all tracks from a file (extract video, audio, subtitle, attachments and other tracks from one file into separate files)
- Fast multi-file workflow (note: no mass/batch export yet)
- Keyboard shortcut workflow
- Losslessly remux video/audio into a different container (file) format
- Take full-resolution snapshots from videos in JPEG/PNG format (low or high quality)
- Export ranges of video frames to images (every nth frame, second, by scene change, best thumbnails)
  - Export only from a selected time range (segment)
  - Optionally include original timestamps in image file names
- Manual input of cutpoint times
- Apply a per-file timecode offset (and auto load timecode from file)
- Edit file metadata, per-track metadata and per-track disposition
- Change rotation/orientation metadata in videos
- View technical data about all tracks
- Timeline zoom and frame/keyframe jumping for cutting around keyframes
- Video thumbnails and audio waveform
- Saves per project cut segments to project file
- View FFmpeg last command log so you can modify and re-run recent commands on the command line
- Undo/redo
- Give labels to cut segments
- Annotate segments with tags
- [Import/export](import-export.md) segments: MP4/MKV chapter marks, Text file, YouTube, CSV, CUE, XML (DaVinci, Final Cut Pro) and more
- MKV/MP4 embedded chapters marks editor
- View subtitles
- Customizable keyboard hotkeys
- Black scene detection, silent audio detection, and scene change detection
- Divide timeline into segments with length L or into N segments or even randomized segments!
- Speed up / slow down video or audio file ([changing FPS](https://github.com/tekintian/lossless-cut/issues/1712))
- Basic [CLI](cli.md) and [HTTP API](api.md)

## Example lossless use cases

- Cut out commercials from a recorded TV show (and re-format from TS to MP4)
- Remove audio tracks from a file
- Extract music track from a video and cut it to your needs
- Add music to a video (or replace existing audio track)
- Combine audio and video tracks from separate recordings
- Include an external subtitle into a video
- Quickly change a H264/H265 MKV video to MOV or MP4 for playback on iPhone
- Import a list of cut times from other tool as a EDL (edit decision list, CSV) and run these cuts with LosslessCut
- Export a list of cut times as a CSV EDL and process these in another tool
- Quickly cut a file by its MP4/MKV chapters
- Quickly cut a [YouTube video](https://youtube-dl.org/) by its chapters (or music times from a comment)
- Change the language of a file's audio/subtitle tracks
- Attach cover art / thumbnail to videos / audio from an external JPEG file or from a frame on the timeline
- Change author, title, GPS position, recording time of a video
- Fix rotation of a video that has the wrong orientation flag set
  - Great for rotating phone videos that come out the wrong way without actually re-encoding the video.
- Loop a video / audio clip X times quickly without re-encoding
  - See [#284](https://github.com/tekintian/lossless-cut/issues/284)
- Convert a video or parts of it into X image files (not lossless)
- Losslessly split a video into one file per scene (note you probably have to shift segments, see [#330](https://github.com/tekintian/lossless-cut/issues/330).)
- Cut away silent parts of an audio/video
- Split video into segments to for example respect Twitter's 140 second limit
- Annotate each segment with one or more tags, then use those tags to organize your segments or use it to create an output folder structure or hierarchy for your segments.
