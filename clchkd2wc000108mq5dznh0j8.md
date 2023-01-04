# Learn HTML: Html "audio" and "video" tag

# 1." HTML Video tag"

The Html video tag is used to embed the video into the browser.

**syntax**: `<video> <sourse src="video link" type="MP4" > </video>`

```xml
<!DOCTYPE html>
<html>
<body>

<video width="320" height="240" controls autoplay muted>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>

</body>
</html>
```

The `<video>` tag contains the height and width attributes.

The "**controls**" inside the video tag define the video controls. We can also use "**autoplay**" to autoplay the video and we can also use "**muted**" to mute the video.

The message between the video tag will be displayed when the video is not displayed.

# 2\. "Audio tag"

The Html audio tag is used to embed the audio into the browser.

**Syntax:** `<audio> <sourse src="link" type="mp3"></audio>`

```xml
<!DOCTYPE html>
<html>
<body>

<audio controls autoplay muted>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

</body>
</html>
```

The "**controls**" inside the video tag define the audio controls. We can also use "**autoplay**" to autoplay the audio and we can also use "**muted**" to mute the audio.

The message between the audio tag will be displayed when the audio is not played.