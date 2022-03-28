# Style Station Plugin

[Install Style Station](https://www.figma.com/community/plugin/909833368999832351/Style-Station)

The Style Station Plugin plugin can take your [SASS](https://blog.logrocket.com/the-definitive-guide-to-scss/) or [LESS](https://tutorialzine.com/2015/07/learn-less-in-10-minutes-or-less) files with CSS rules and create the same styles in Figma. Or update the existing.
Currently it can supports only text and paint styles. But also it can operates with layers.

### [Check this article](https://medium.com/@max_39664/style-station-5d5e81998e33) to get a detailed overview with examples.
### You can support the development [here](https://paypal.me/maxbazarov)

<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/apply-upload.png"/>
<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/apply-edit.png"/>
<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/apply-files.png"/>
<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/apply-edit-cloud.png"/>
<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/imported.png"/>

Also Style Station can export styles from Figma to SASS or LESS file.

<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/export.png"/>

## Currently supported styles:

```less
.TextStyle {
  font-size:                  10px; // OR 10
  font-family:                Times;
  font-weight:                Regular;
  line-height:                100%; // OR 10px OR 1.2 (multiplier for font-size) OR AUTO
  letter-spacing:             100%; // OR 10px  
  text-decoration:            underline;// OR line-through  
  text-indent:                32px;
  text-transform:             uppercase;  // "uppercase", "lowercase","title"(Figma custom), "none"
}
.PaintStyle{
  background-color:           red;   //  #FF00FF;
}
#Rectangle{
  border-color:               blue; 
  border-color:               red; 
  border-width:               10px;
  background-color:           red;   //  #FF00FF; 
  -pt-border-update:          true;  // Use it if you want to replace existing borders, instead of adding a new one
}
#Group{
  padding:                    10px; // currently only one value for left,right,top and bottom
}
```
## Supported Targets
You can update the following Figma objects.

```less
// Update style
.MyStyles .Group .TextLarge{
    font-size:                40px;
}

// Update any layer properties inside a frame or component
#MyFrame .Back{
  border-color:         blue; 
  border-width:         10px;
  background-color:     #FFFFFF;
}
// Or update any group node itself
#My__Component{
  padding: 10px; // OR 10px 10px  OR 10px 20px 30px OR 10px 10px 20px 20px
  pagging-top: 10px;
  pagging-left: 10px;
  pagging-bottom: 10px;
  pagging-right: 10px;
}
```

## Community
[Github Discussions](https://github.com/MaxBazarov/style-station-plugin/discussions)
