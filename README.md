<div align="center">

## Force browser to reload or refresh


</div>

### Description

How do I force a reload/refresh from the current page?

Found at http://www.irt.org
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Found on the Web](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/found-on-the-web.md)
**Level**          |Unknown
**User Rating**    |4.6 (23 globes from 5 users)
**Compatibility**  |
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__2-68.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/found-on-the-web-force-browser-to-reload-or-refresh__2-180/archive/master.zip)





### Source Code

You can for JavaScript 1.1 use the location objects reload method:
<FORM>
<INPUT TYPE="BUTTON" onClick="window.location.href.reload()" VALUE="Reload">
</FORM>
Failing that you could try a meta tag that doesn't allow the page to be cached so that the following would reload:
<FORM>
<INPUT TYPE="BUTTOM" onClick="window.location.href=window.location.href">
</FORM>
The no cache meta tag needs to be placed in between the <HEAD> and </HEAD> tags:
<META HTTP-EQUIV="no-cache">
Or you could use the meta tag for expires, to always ensure that a newer copy is loaded:
<META HTTP-EQUIV="expires" CONTENT="Wed, 26 Feb 1997 08:21:57 GMT">
Or you could refresh the page automatically after a delay using the refresh meta:
<META HTTP-EQUIV="Refresh" CONTENT="3;URL=http://www.some.org/some.html">

