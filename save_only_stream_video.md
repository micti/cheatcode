You're watching only streaming video (ts), and you want to view offline...

### Common steps

- Select HD 1080 / 720 ...
- Check all files in playlist (.m3u8)
- Create batch download for Download Manager (IDM, Flashget, iGetter...)
- Create file list after download
- Join all files with ``ffmpeg concat`` demuxer command ``ffmpeg -f concat -safe 0 -i mylist.txt -c copy a.ts``

### References
- https://superuser.com/questions/979633/how-to-split-and-join-without-transcoding-avc-mpeg-ts-video-files-in-windows-wit
- https://trac.ffmpeg.org/wiki/Concatenate
