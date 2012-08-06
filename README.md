## spriteOnHover
[spriteOnHover](http://apolinariopassos.com.br/dev/spriteonhover-jquery-plugin/) is a lightweight jQuery plugin designed to **animate** your sprites on **hover** (duh). 

## Instalation
Include script *after* the jQuery library (unless you are packaging scripts somehow else):
`<script src="/path/to/jquery.spriteOnHover-0.2.5.min.js"></script>`

## Simplest Usage
    $('#yourSprite').spriteOnHover();

This will make the plugin work this the default parameters, which points to this:

    $('#yourSprite').spriteOnHover({fps:30, orientation:’horizontal’, rewind: true, loop: false, autostart:false;repeat:true});

The usage is just hovering the sprite, you set `$('#yourSprite').spriteOnHover();` and the element `'#yourSprite'` will be turned into a hoverable sprite, no need to use the `mouseover`, `mouseenter`, `mouseleave` or `hover` events of jquery.
	
## The CSS
    #yourSprite{
	    width: 43px; //Your sprite width
	    height: 43px; //Your sprite height
	    background: transparent url(path/to/your/spritesheet.png) 0px 0px no-repeat; //Path to your spritesheet
    }

**Attention**: The spriteOnHover plugin will autodetect how many frames your sprite has, based on the orientation parameter, but it’s crucial that every frame has the exactly same size as the others. For now, multi-line sprites are not supported.

## The parameters
spriteOnHover has 6 parameters:

* fps: Integer - The frame-per-second count of your animation (Default: 30)

*   orientation: Possible values: `"horizontal"` or `"vertical"` - The orientation of your spritesheet, for now, the plugin supports only a single-orientated spritesheet, and can’t handle multidimensional sprites. (Default: `"horizontal"`). Example:
    * [This](http://apolinariopassos.com.br/images/explosion-spritesheet.png) is a horizontal spritesheet
    * [This](http://apolinariopassos.com.br/dev/images/btn-seta-clientes-spritesheet-vert.png) is a vertical spritesheet
    * [This](http://apolinariopassos.com.br/dev/images/multi-line-animation.jpg) is a multi-line spritesheet (not supported for now)


*   rewind: Possible values: `true`, `false` or `"unanimate"` - Is how your animation should work on mouseleave: 
                                                           
    * `true`: the animation will be animatedly rewinded;
    * `false`: the animation will stop in the last frame;
    * `"unanimate"`: the sprite will go back straight to the first frame, with no animation 
    * (Default: `true`)                                                      

*   loop: Possible values: `true`, `false` or `"infinite"`
    * `false`, your animation will be displayed once, 
    * `true`, your animation will be looped
    * `"infinite"`, after it’s started, you will get an infinitely looping animation that is no longer controlled by the hover action; 
    * (default: `false`)

*   autostart: Possible values: `true` or `false` - Determines if your animation will autostart or only be triggered by hover.
    * `true`: the animation will start without a hover event 
    * `false`: the animation will only start with on mouseover 
    * (default: `false`)

*   repeat: Possible values: `true` or `false`
    * `true`: the animation will be triggered every time you hover the sprite (of course after finishing the last event)
    * `false`, the animation will be triggered only at the first hover action and after that will get stuck at the last frame of your animation. 
    * (deafult: `true`); 

## Demos & Examples
In the plugin's [page](http://apolinariopassos.com.br/dev/spriteOnHover/demo/)

## Donate
Want to help me get the TODO features faster or the plugin just solved your problem? 
[Donate](http://www.apolinariopassos.com.br/donate) <3


## License

                DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                        Version 2, December 2004

    Everyone is permitted to copy and distribute verbatim or modified
    copies of this license document, and changing it is allowed as long
    as the name is changed.

                DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
      TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

    0. You just DO WHAT THE FUCK YOU WANT TO.	