# Fork of [TheFrenchGhosty's YouTube-DL Archivist Scripts](https://gitlab.com/TheFrenchGhosty/TheFrenchGhostys-YouTube-DL-Archivist-Scripts)

**Requires [youtube-dl](https://youtube-dl.org/) and [ffmpeg](https://www.ffmpeg.org/)**

The ultimate collection of scripts for YouTube-DL


## Usage :

Install [youtube-dl](https://youtube-dl.org/) and [ffmpeg](https://www.ffmpeg.org/)

Create a folder where you want your videos downloaded in a drive where you have Gigabytes/Terabytes of space available 

## Archive, Active and Watch Scripts?

This repository got rid of this weirdness. Just add a URL to the source file either in channels, playlists or single videos and run the scripts.

# Details : 

`--format "(bestvideo[vcodec=av01][height>=4320][fps>30]/bestvideo[vcodec=vp9.2][height>=4320][fps>30]/bestvideo[vcodec=vp9][height>=4320][fps>30]/bestvideo[vcodec=av01][height>=4320]/bestvideo[vcodec=vp9.2][height>=4320]/bestvideo[vcodec=vp9][height>=4320]/bestvideo[height>=4320]/bestvideo[vcodec=av01][height>=2880][fps>30]/bestvideo[vcodec=vp9.2][height>=2880][fps>30]/bestvideo[vcodec=vp9][height>=2880][fps>30]/bestvideo[vcodec=av01][height>=2880]/bestvideo[vcodec=vp9.2][height>=2880]/bestvideo[vcodec=vp9][height>=2880]/bestvideo[height>=2880]/bestvideo[vcodec=av01][height>=2160][fps>30]/bestvideo[vcodec=vp9.2][height>=2160][fps>30]/bestvideo[vcodec=vp9][height>=2160][fps>30]/bestvideo[vcodec=av01][height>=2160]/bestvideo[vcodec=vp9.2][height>=2160]/bestvideo[vcodec=vp9][height>=2160]/bestvideo[height>=2160]/bestvideo[vcodec=av01][height>=1440][fps>30]/bestvideo[vcodec=vp9.2][height>=1440][fps>30]/bestvideo[vcodec=vp9][height>=1440][fps>30]/bestvideo[vcodec=av01][height>=1440]/bestvideo[vcodec=vp9.2][height>=1440]/bestvideo[vcodec=vp9][height>=1440]/bestvideo[height>=1440]/bestvideo[vcodec=av01][height>=1080][fps>30]/bestvideo[vcodec=vp9.2][height>=1080][fps>30]/bestvideo[vcodec=vp9][height>=1080][fps>30]/bestvideo[vcodec=av01][height>=1080]/bestvideo[vcodec=vp9.2][height>=1080]/bestvideo[vcodec=vp9][height>=1080]/bestvideo[height>=1080]/bestvideo[vcodec=av01][height>=720][fps>30]/bestvideo[vcodec=vp9.2][height>=720][fps>30]/bestvideo[vcodec=vp9][height>=720][fps>30]/bestvideo[vcodec=av01][height>=720]/bestvideo[vcodec=vp9.2][height>=720]/bestvideo[vcodec=vp9][height>=720]/bestvideo[height>=720]/bestvideo)+(bestaudio[acodec=opus]/bestaudio)/best"` : Courtesy of [Veloldo](https://redd.it/c6fh4x), tell youtube-dl to download the best quality available prioritizing the most compressed/recent codecs

`--verbose` : Tell youtube-dl to print various debugging information

`--force-ipv4` : Tell youtube-dl to use IPv4, needed because lots of hosting and VPNs providers don't support IPv6.

`--ignore-errors` : Tell youtube-dl to continue on download errors (for example to skip unavailable videos in a playlist)

`--no-continue` : Tell youtube-dl not to resume partially downloaded files and to restart from the beginning (Mainly to avoid corruption)

`--no-overwrites` : Tell youtube-dl not to overwrite existing files (Useful when metadata has already been downloaded)

`--download-archive archive.log` : Tell youtube-dl to write every video that has been downloaded in `archive.log` to automatically skip them next time the script is started

`--add-metadata` : Tell youtube-dl to write metadata to the video files

`--write-description` : Tell youtube-dl to write video description to a `.description` file

`--write-info-json` : Tell youtube-dl to write video metadata to a `.info.json` file

`--write-annotations` : Tell youtube-dl to write video annotations to a `.annotations.xml` file

`--write-thumbnail` : Tell youtube-dl to write thumbnail image to disk

`--embed-thumbnail` : Tell youtube-dl to embed thumbnail in the audio as cover art (only useful when downloading audio-only content like podcast)

`--all-subs` : Tell youtube-dl to download all the available subtitles of the video

`--sub-format "srt"` : Tell youtube-dl to prioritize `.srt` subtitles

`--embed-subs` : Tell youtube-dl to embed subtitles in the video
