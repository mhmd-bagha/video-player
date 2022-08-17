# video-player

a video player create by mhmd-bagh 


# use video player

require file video-player.css to tag header
```
<link rel="stylesheet" href="./css/video-player.css">
```
require file video-palyer.js to tag end body
```
<script src="./js/video-player.js"></script>
```

# add tag video
```
<video id="video-player" class="video-player">
        <source src="<Video Address>"
                type="video/mkv">
        Your browser does not support the video tag.
    </video>
```

# a create new object VideoPlayer

```
<script>
    window.onload = ()=>{
        let video_player = new VideoPlayer({
            selector: "#video-player",
            config: {
                storage: {
                    captionOffset: false,
                    playerSpeed: false,
                    captionSize: false
                },
            }
        })
    }
</script>
```
or use jquery
## require jquery cdn 
``` <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script> ```
and
```
    $(document).ready(()=>{
        let video_player = new VideoPlayer({
            selector: "#video-player",
            config: {
                storage: {
                    captionOffset: false,
                    playerSpeed: false,
                    captionSize: false
                },
            }
        })
    })
</script>
```
