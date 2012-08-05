## SpriteOnHover
spriteOnHover is a lightweight (2.51KB) jQuery plugin is designed to **animate** your sprites on **hover** (duh). 

## Instalation
Include script *after* the jQuery library (unless you are packaging scripts somehow else):
    <script src="/path/to/jquery.spriteOnHover-0.2.5.js"></script>

## Simplest Usage
    $('#yourSprite').spriteOnHover();

This will make the plugin work this the default parameters, which points to this:
    $('#yourSprite').spriteOnHover({fps:30, orientation:�horizontal�, rewind: true, loop: true, autostart:false;repeat:true});

The usage is just hovering the sprite, you set `$('#yourSprite').spriteOnHover();` and the element `'#yourSprite'` will be turned into a hoverable sprite, no need to use the `mouseover`, `mouseenter`, `mouseleave` or `hover` events of jquery.

## The CSS
    #yourSprite{
	    width: 43px; //Your sprite width
	    height: 43px; //Your sprite height
	    background: transparent url(path/to/your/spritesheet.png) 0px 0px no-repeat; //Path to your spritesheet
    }

Attention: The spriteOnHover plugin will autodetect how many frames your sprite has, based on the orientation parameter, but it�s crucial that every frame has the exactly same size as the others. For now, multi-line sprites are not supported.

## The parameters
spriteOnHover has 6 parameters:

- fps: Integer - The frame-per-second count of your animation (Default: 30)

- orientation: Possible values: �horizontal� or �vertical� - The orientation of your spritesheet, for now, the plugin supports only a single-orientated spritesheet, and can�t handle multidimensional sprites. (Default: �horizontal�);
Example: 
*[This](http://apolinariopassos.com.br) is a horizontal spritesheet
*[This](http://apolinariopassos.com.br) is a vertical spritesheet
*[This](http://apolinariopassos.com.br) is a multi-line spritesheet (not supported for now)

- rewind: Possible values: true, false or �unanimate� - How your animation should work on mouseleave: 
true: the animation will be animatedly rewinded; 
false: the animation will stop in the last frame;
�unanimate�: the sprite will go back straight to the first frame, with no animation
(Default: True);

- loop: Possible values: true, false or �infinite� - If false, your animation will be displayed once, if true, your animation will be looped, if �infinite�, after it�s started, you will get an infinitely looping animation that is no longer controlled by the hover action; (default: false)

- autostart: Possible values: true or false - Determines if your animation will autostart or only be triggered by hover. If true, the animation will, for the first time, start without a hover event and will 
be animated (default: false)

- repeat: Possible values: true or false - If true, the animation will be triggered everytime you hover the sprite (of course after finishing the last event), if false, the animation will be triggered only at the first hover action and after that will get stuck at the last frame of your animation. (deafult: true); 

## Demo & (lots of) Examples
In the plugin's [page](http://www.apolinariopassos.com.br)

## License

                DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                        Version 2, December 2004

    Everyone is permitted to copy and distribute verbatim or modified
    copies of this license document, and changing it is allowed as long
    as the name is changed.

                DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
      TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

    0. You just DO WHAT THE FUCK YOU WANT TO.	