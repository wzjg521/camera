<!doctype html>
<html lang="en">
<head>
    <title>WebRTC tutorial</title>
    <!-- http://www.webrtc.org/ -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, user-scalable=no, minimum-scale=1.0, maximum-scale=1.0">
</head>
<body>

<p id="errorMessage"></p>
<center>
<video id="monitor" autoplay width="500px" style="visibility: visible;"></video>
<img id="img" width="500px"/>
</center>
<canvas style="display:none" id="canvas"></canvas>

<button id="snap">拍照</button>

<script>
    navigator.getUserMedia = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia;
    window.URL = window.URL || window.webkitURL;
    var camvideo = document.getElementById('monitor');
    if (!navigator.getUserMedia)
    {
        document.getElementById('errorMessage').innerHTML =
            'Sorry. <code>navigator.getUserMedia()</code> is not available.';
    }
    navigator.getUserMedia({video: true}, gotStream, noStream);
    function gotStream(stream)
    {
        if (window.URL)
        {   camvideo.src = window.URL.createObjectURL(stream);   }
        else // Opera
        {   camvideo.src = stream;   }
        camvideo.onerror = function(e)
        {   stream.stop();   };
        stream.onended = noStream;
    }
    function noStream(e)
    {
        var msg = 'No camera available.';
        if (e.code == 1)
        {   msg = 'User denied access to use camera.';   }
        document.getElementById('errorMessage').textContent = msg;
    }
    document.getElementById('snap').onclick=function () {
        var video = document.getElementById("monitor");//获取前台要截图的video对象，
        var canvas = document.getElementById('canvas');//获取前台的canvas对象，用于作图
        var ctx = canvas.getContext('2d');//设置canvas绘制2d图，
        canvas.width = video.videoWidth;
        canvas.height = video.videoHeight;
        ctx.drawImage(video, 0, 0, video.videoWidth, video.videoHeight);//将video视频绘制到canvas中
        var images = canvas.toDataURL('image/png');//canvas的api中的toDataURL（）保存图像
        document.getElementById('img').src=images;
    };
</script>
</body>
</html>
