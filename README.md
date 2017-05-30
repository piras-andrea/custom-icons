Custom svg-icons based on  [Font Awesome Cheatsheet](http://fontawesome.io/cheatsheet/) 

## How to generate new svg-based font

- Install Font Awesome on your system. See this [youtube video](https://www.youtube.com/watch?v=tGs_omrgeBk)
- Install [Inkscape](https://inkscape.org/it/download/)
- Open Inkscape, select FontAwesome as font, create layer, insert new text, copy icon from FontAwesome's cheatsheet and paste.
- Create new layer and paste another icon just like above
- Do this operations; bear in mind that you might need to apply differenct, intersection ecc operations on your objects.

   Group objects (Object -> Group Object (ctrl-g))  
   Edit -> Resize page to selection (MAIUSC-CTRL-R)  
   Path -> From Object to path Tracciato -> (MAIUSC-CTRL-C)  
   
- Save your new svg
- Go to [Icomoon](https://icomoon.io/app)
- **Import your font** (in svg format), then (__and just then__) import all your new svg icons and download new generated font's zipfile
- Substitute files in your project:

```
 rm icomoon.eot icomoon.svg icomoon.ttf icomoon.woff && unzip.exe icomoon.zip && mv fonts/* . && rm
-r demo-files demo.html Read\ Me.txt selection.json style.css fonts/
```

- Create your classes (icomoon suggests you the code you need):
 
 ```
.farx-associate-document-2:before {
  content: "\e90b";
}
 ```
 
 - Test your results
