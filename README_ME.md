### ref
- https://github.com/crisbal/album-splitter
- https://github.com/ytdl-org/youtube-dl
- https://gist.github.com/umidjons/8a15ba3813039626553929458e3ad1fc
  - for best quality of audio file
- https://stackoverflow.com/a/60158194/11681543

### attention
- yt command not work (about --no-check-certificate)

## 1. download youtube to mp3 by myself
```
youtube-dl -i --extract-audio --audio-format mp3 --audio-quality 0 --no-check-certificate <youtube-link>
```
or (not tried yet)
```
youtube-dl -i --extract-audio --audio-format mp3 --audio-quality 0 --no-check-certificate --config-location "./album.mp3" <youtube-link>
```

## 2. add track info in tracks.txt

## 3. (after download) split albums
```
python -m album_splitter --file ./album.mp3 --album "<album-title>" --artist "<artist>"
```
