<!DOCTYPE html>
<meta http-equiv="Content-Type" content="text/html;charset=utf-8" >
<html >
<head>
  <title>Teste navegador</title>
</head>
<body onload="identifyBrowser()">
  
 
  <div id="mediaPlayer" >
    <EMBED TYPE="application/x-mplayer2" SRC="Jack_Sparrow-Violino.mp3" NAME="MediaPlayer"
    WIDTH="192" HEIGHT="45" ShowControls="1" ShowStatusBar="0" ShowDisplay="0" autostart="1"> </EMBED>
  </div>

  <div id="html5">    
   <audio controls>
    <source src="Jack_Sparrow-Violino.mp3" type="audio/mp3">      
        Your browser does not support the audio element.
      </audio> 

    </div>

 <SCRIPT Language="Javascript">
  function identifyBrowser() {
    var ua = navigator.userAgent.toLowerCase();
    if (ua.indexOf("msie") != -1) {        
         document.getElementById('html5').style.display = "none";
    } else{     
     var d = document.getElementById('mediaPlayer').style.display = "none";     
    }
  }
 
  </SCRIPT>


</body>
</html>
