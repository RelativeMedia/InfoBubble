### Description
Clone of Google Maps InfoBubble Library by **Luke Mahe** and **Chris Broadfoot** with some optimizations and new features.

### New Features

  * Active Tab CSS Class Definition
  * Tab Padding Definition
    * Default tab padding is set to 10px, like the InfoBubble
  * Removed the outerArrow lockout for no borderWidth
  

### Documentation
The new features can be defined the same way all the other options are defined by adding them when you call a new `InfoBubble` class.
#### Defining an active tab class

```Javascript
infoBubble2 = new InfoBubble({
    position: myLatlng,
    minWidth: 240,
    minHeight: 220,
    shadowStyle: 1,
    padding: 0,
    /**
     * Padding around the tabs, now set seperately
     * from the InfoBubble padding
     **/
    tabPadding: 12,
    /** 
     * You can set the background color to transparent, 
     * and define a class instead
     **/
    backgroundColor: 'transparent',
    borderRadius: 4,
    arrowSize: 10,
    borderWidth: 0,
    /**
     * Now that there is no borderWidth check, 
     * you can define a borderColor and it will 
     * apply to Just the arrow
     **/
    borderColor: '#AB2424',
    disableAutoPan: true,
    hideCloseButton: false,
    arrowPosition: 30,
    /** 
     * use the .phoney class to define all styling 
     * for your InfoBubble
     **/
    backgroundClassName: 'phoney',
    /**
     * define a CSS class name for all, this is 
     * technically the "inactive" tab class
     **/
    tabClassName: 'tabClass',
    /**
     * define a CSS class name for active tabs only
     **/
    activeTabClassName: 'activeTabClass',
    arrowStyle: 0
  });
```