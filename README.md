Custom svg-icons based on  [Font Awesome Cheatsheet](http://fontawesome.io/cheatsheet/) 

## How to generate new svg-based font

- Install [Inkscape](https://inkscape.org/it/download/)
- Install Font Awesome on your system. See this [youtube video](https://www.youtube.com/watch?v=tGs_omrgeBk)
- Open Inkscape, select FontAwesome as font, create layer, insert new text, copy icon from FontAwesome's cheatsheet and paste.
- Create new layer and paste another icon just like above
- Do this operations; bear in mind that you might need to apply 'difference', 'intersection' ecc operations on your objects.

   Group objects (Object -> Group Object (ctrl-g))  
   Edit -> Resize page to selection (MAIUSC-CTRL-R)  
   Path -> From Object to path Tracciato -> (MAIUSC-CTRL-C)  
   
- Save your new svg
- Go to [Icomoon](https://icomoon.io/app)
- **Import your font** (in svg format), then (_and just then_) import all your new svg icons and download new generated font's zipfile (you can't have multicolor icons; if icomoon reports that some of your icons are multicolor, you might need to fix your icon)
- Substitute files in your project:

```
 rm icomoon.eot icomoon.svg icomoon.ttf icomoon.woff && unzip.exe icomoon.zip && mv fonts/* . && rm
-r demo-files demo.html Read\ Me.txt selection.json style.css fonts/
```

- Check that codes for old icons are not changed
- Create your classes (icomoon suggests you the code you need):
 
 ```
.farx-associate-document-2:before {
  content: "\e90b";
}
 ```
 
 - Test your results
