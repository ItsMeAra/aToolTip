# [aToolTip][1]

[DOWNLOAD][2] [DEMO][3] 

## Quick Facts

*   Lightweight (only 3kb uncompressed)
*   Easy to use
*   Choice of fixed, on click or follow mouse tooltip
*   Highly customizable
*   Compatable with Firefox 2.5+, Safari, Opera, Chrome and Internet Explorer 6, 7 & 8

  

## Demos

*   [Normal Tooltip][4] - This is a normal tooltip with default settings.
*   [Fixed Tooltip][4] - This is a fixed tooltip that doesnt follow the mouse.
*   [On Click Tooltip][1] - This is a click activated tooltip with content passed in from 'tipContent' param
*   [Callback Tooltip][4] - This is a click activated tooltip with callback functions.

## Usage

Start off by including jQuery as well as the aToolTip plugin

    
    
    
    

Initiate the plugin

    // initiate the plugin after DOM has loaded
    $(function(){
    
    	// basic usage
    	$('a.normalTip').aToolTip();
    	
    	// fixed tooltip
    	$('a.fixedTip').aToolTip({
    		fixed: true
    	});
    	
    	// on click tooltip with custom content
    	$('a.clickTip').aToolTip({
    		clickIt: true,
    		tipContent: 'Hello I am aToolTip with content from param'
    	});	
    	
    	// List of all paramaters and their default values:
    	$('a').aToolTip({
    		clickIt: false, 					// set to true for click activated tooltip
    		closeTipBtn: 'aToolTipCloseBtn',	// you can set custom class name for close button on tooltip
    		fixed: false,						// Set true to activate fixed position
    		inSpeed: 400,						// Speed tooltip fades in
    		outSpeed: 100,						// Speed tooltip fades out
    		tipContent: '',						// Pass in content or it will use objects 'title' attribute
    		toolTipClass: 'aToolTip',			// Set custom class for tooltip
    		xOffset: 5,							// x Position
    		yOffset: 5,							// y position
    		onShow: null,						// Callback function on show
        	onHide: null						// Callback function on hide
    	});
    	
    });
    

Basic HTML markup used in the demos

    
    [Normal Tooltip][4]
    [Fixed Tooltip][4]
    [On Click Tooltip][1]
    

What does the tooltip markup look like?

 [1]: #
 [2]: https://github.com/AraLA22/aToolTip "Download from Github"
 [3]: #demos
 [4]: # "Hello, I am aToolTip"