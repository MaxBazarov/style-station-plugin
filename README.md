# Style Station Plugin

https://www.figma.com/community/plugin/909833368999832351/Style-Station

Style Station Plugin (ex-Figmass) plugin can take your SASS or LESS files with CSS rules and create the same styles in Figma. Or update the existing.
Currently it can supports only text and paint styles. 

<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/import.png"/>
<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/imported.png"/>

Also Style Station can export styles from Figma to SASS or LESS file.

<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/export.png"/>

## Currently supported styles:

```css
.TextStyle {
  font-size:                  10px; // OR 10
  font-family:                Times;
  font-weight:                Regular;
  line-height:                100%; // OR 10px;
  letter-spacing:             100%; // OR 10px  
  text-decoration:            underline;// OR line-through  
  text-indent:                32px;
  text-transform:             uppercase;  // "uppercase", "lowercase","title"(Figma custom), "none"
}
.PaintStyle{
  background-color:           red;   //  #FF00FF;
}
```
## Supported Targets
You can update the following Figma objects.

```css
// Update style
.MyStyles .Group .TextLarge{
    font-size:                40px;
}

// Update any node properties
#MyWidgets #Buttons #Submit{
    .Back{
        background-color: #FFFFFF;
    }
}

## Community
https://github.com/MaxBazarov/style-station-plugin/discussions
