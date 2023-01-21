# Fix-chrome-play-local-music-can-not-fast-forward-and-back-forward



```
var theVideo = document.getElementByTagName("video");
  document.onkeydown = function(event) {
      switch (event.keyCode) {
         case 37:
              event.preventDefault();
              
              vid_currentTime = theVideo.currentTime;
              theVideo.currentTime = vid_currentTime - 5;
            break;
         
         case 39:
              event.preventDefault();
              
              vid_currentTime = theVideo.currentTime;
              theVideo.currentTime = vid_currentTime + 5;
            break;
         
      }
  };
```