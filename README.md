<div align="center">

## Downloading Web Page HTML Example


</div>

### Description

This code demonstrates how to download the HTML source code from a specified web page and output it to the screen. Can be used to retrieve tags, or words, or peanut butter from web pages. Enjoy.
 
### More Info
 
Blindness?


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[C\.V\.](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/c-v.md)
**Level**          |Intermediate
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |Java \(JDK 1\.1\), Java \(JDK 1\.2\)
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__2-68.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/c-v-downloading-web-page-html-example__2-3906/archive/master.zip)





### Source Code

```
import java.net.*;
import java.io.*;
public class URL1
{
  public static void main(String[] args) throws Exception {
    URL url = new URL("http://www.coryvia.net");
    InputStream html = url.openStream();
    int c = 0;
    String a = "";
    while(c != -1) {
      a = "";
      c = html.read();
      if(c == (char)60) {
        while(c != (char)62) {
          a = a + (char)c;
          c = html.read();
        }
      }
      if(a == "") {}
      else
        System.out.println(a + ">");
    }
  }
}
```

