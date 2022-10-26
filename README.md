# Style Station Plugin

[Install Style Station](https://www.figma.com/community/plugin/909833368999832351/Style-Station)

The Style Station Plugin plugin can take your [SASS](https://blog.logrocket.com/the-definitive-guide-to-scss/) or [LESS](https://tutorialzine.com/2015/07/learn-less-in-10-minutes-or-less) files with CSS rules and create the same styles in Figma. Or update the existing.
Currently it can supports only text and paint styles. But also it can operates with layers.

### [Check this article](https://medium.com/@max_39664/style-station-5d5e81998e33) to get a detailed overview with examples.

<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/apply-upload.png"/>
<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/apply-edit.png"/>
<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/apply-files.png"/>
<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/apply-edit-cloud.png"/>
<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/imported.png"/>

Also Style Station can export styles from Figma to SASS or LESS file.

<img width="755" src="https://raw.githubusercontent.com/MaxBazarov/style-station-plugin/master/screenshots/export.png"/>

## Currently supported CSS style:

```css
// FOR FIGMA TEXT STYLES
.TextStyle {
  font-size:                  10px; // OR 10
  font-family:                Times;
  font-weight:                Regular;
  line-height:                100%; // OR 10px OR 1.2 (multiplier for font-size) OR AUTO
  letter-spacing:             100%; // OR 10px  
  text-decoration:            underline;// OR line-through  OR none
  text-indent:                32px;
  text-transform:             uppercase;  // "uppercase", "lowercase","title"(Figma custom), "none"
  text-indent:                100;  // The indentation of paragraphs (offset of the first line from the left). 
  -pt-paragraph-spacing:      12;  // The vertical distance between paragraphs
  text-align:                 left; // left OR right OR center OR justify !!
                                    // Not a text sttyle property actually, so it will be applied to 
                                    // text nodes which the selected style assigned to
}
// FOR FIGMA PAINT STYLES
.PaintStyle{
  background-color:           red;   //  #FF00FF;
  OR
  color:                      red;   //  #FF00FF;
}
// FOR STANDALONE FRAMES, SHAPES, RECTANGLES NODES
#Rectangle{
  border-color:               blue; 
  border-color:               red; 
  border-width:               10px;
  background-color:           red;   //  #FF00FF;   
  -pt-border-update:          true;  // Use it if you want to replace existing borders, instead of adding a new one
  border-radius:              5px; // set for all corners
  border-radius:              1px 2px 3 4; // top-left top-right  bottom-right  bottom-left 
  border-radius:              1px 2px 3px; //  top-left top-right-and-bottom-left  bottom-right
  border-radius:              1px 2px; //  top-left-and-bottom-right | top-right-and-bottom-left
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

// Update any  node properties
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

## Color definition types
{
  background-color:  #FF00FF;
  background-color:  #FF00FFBB;
  background-color:  blue;
  background-color:  hsla(240,100%,50%,0.5);
  background-color:  hsl(240,100%,50%);
  background-color:      linear-gradient(45deg, #000000,#B0AFB4);
  background-color:      linear-gradient(134deg, #004B3A 0%, #2D8B61 51%, #9BD77E 100%);
}


## Community
[Github Discussions](https://github.com/MaxBazarov/style-station-plugin/discussions)
