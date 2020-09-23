<div align="center">

## Right Click Disabler


</div>

### Description

This is a Javascript code that disables right clicks in I.E. and Netscape. If you like it please rate it. Good Luck.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Robert Long](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/robert-long.md)
**Level**          |Intermediate
**User Rating**    |4.5 (18 globes from 4 users)
**Compatibility**  |
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__2-68.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/robert-long-right-click-disabler__2-2042/archive/master.zip)





### Source Code

```
<SCRIPT LANGUAGE="Javascript">
document.onmousedown=click;
if (document.layers) window.captureEvents(Event.MOUSEDOWN); window.onmousedown=click;
function click(e){
	if (navigator.appName.indexOf("Netscape") != -1){
		//alert(e.which);
		if (e.which != '1'){
			return false;
		}
	}
	if (navigator.appName.indexOf("Explorer") != -1){
		//alert(event.button);
		if (event.button != '1'){
			alert("Right click has been disabled.");
			return false;
		}
	}
}
</SCRIPT>
```

