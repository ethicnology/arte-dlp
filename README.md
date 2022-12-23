# arte-dlp

## deprecated

Please [read this issue](https://github.com/yt-dlp/yt-dlp/issues/5853)
With the [custom fork of ffmpeg by yt-dlp](https://github.com/yt-dlp/FFmpeg-Builds) this script can can be useless using only this command:

```sh
yt-dlp --embed-subs --sub-langs all --convert-subs srt --ppa "EmbedSubtitle:-disposition:s:0 0" --merge mkv "URL"
```

## motivation

Many websites uses WebVTT (.vtt) subtitles that are not recognized by media center softwares or the rendering does not display well.
For the given URL this program will download video, audio and all available subtitles, if the subtitles are WebVTT (.vtt) encoded it will convert them into SubRip (.srt) before merging them all in a Matroska (.mkv) container.

## prerequisites

- python3
- yt-dlp
- ffmpeg

## install

Download the script

```sh
wget https://raw.githubusercontent.com/ethicnology/arte-dlp/main/arte-dlp
```

Add it to your path

```sh
sudo mv arte-dlp /usr/local/bin
```

Make it executable

```sh
sudo chmod +x  /usr/local/bin/arte-dlp
```

## usage

```sh
arte-dlp URL
```

![demo](https://raw.githubusercontent.com/ethicnology/arte-dlp/main/demo.gif)

## websites

Here is a list of websites that work well with it, please do an issue/PR if you try this tool and it works on any other website.

- [arte.tv](https://www.arte.tv)
