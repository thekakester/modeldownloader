* In chrome, press Ctrl+Shift+i to open developer mode.
* Click the "Console" tab.
* Paste the following code into the input, then press enter

```
function d(e){if(e.geometry){for(var t=e.geometry.f.array,o=e.geometry.attributes.position.array,r=0;r<t.length;r+=3)b+="f "+(t[r]+c)+" "+(t[r+1]+c)+" "+(t[r+2]+c)+"%0A";for(var r=0;r<o.length;r+=3)a+="v "+Math.round(1e6*o[r])/1e6+" "+Math.round(1e6*o[r+1])/1e6+" "+Math.round(1e6*o[r+2])/1e6+"%0A",c++}for(var r=0;r<e.children.length;r++){var n=e.children[r];d(n)}}var a="",b="",c=1;confirm("Did you save?\nRunning this script will take you away from this window.\nClick ok to continue or cancel to do nothing")&&(d(CK.activeCharacter.threeObj),document.write("<a id='mitchrocks' style='display:none' href='data:text/html,"+a+"%0A"+b+"' download='model.obj'>Click here to download your model</a>Your model is downloading!<br>You can use an online model viewer line <a href='https://3dviewer.net/'>3dviewer.net</a> to check it out!"),document.write("<script>document.getElementById('mitchrocks').click()</script>"));
```
