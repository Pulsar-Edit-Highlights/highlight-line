
# Customization

Colors can be set by modifying the  [`Theme.less`]  
stylesheet or by adding to your  `style.less`  file.

<br>

*Using the  `.cursor-line`  class selector is not recommended as  
you will loose highlighting when selecting text on the current line.*

<br>

```scss
atom-text-editor::shadow {
    
    /*
     *  Ｂａｃｋｇｒｏｕｎｄ
     *  Uses !important to override theme specific settings
     */
    
    .line.highlight-line {
        background : rgba( 255 , 0 , 0 , 0.3 ) !important ;
    }

    /*
     *  Ｕｎｄｅｒｌｉｎｅ
     *  Replace `solid` with `dashed` or `dotted` depending
     *  on the style you selected in the settings.
     */
    
    .line.highlight-line-multi-line-solid-bottom {
        border-bottom-color : red ;
    }

    /*
     *  Ｂｏｒｄｅｒｓ
     *  Style for the optional area selection borders.
     */
    
    .line.highlight-line-multi-line-solid-top {
        border-top-color : red ;
    }
}
```

<br>

[`Theme.less`]: ../Resources/Styles/Theme.less
