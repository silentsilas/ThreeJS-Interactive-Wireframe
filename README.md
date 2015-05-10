# ThreeJS-Interactive-Wireframe
Trippy visuals are to be had with the help of sine functions, Dat.GUI, and Three.js.

## Instructions

* Go to the [Site](http://poeticode.github.io/ThreeJS-Interactive-Wireframe/) in a modern browser.
 * Should also work on smart phones.
* Zoom in and out with the mousewheel. Smart phones can't zoom currently.
* Click on the two small objects to toggle their wireframe.
* Adjust the sliders to animate the giant bumpy sphere in weird ways.
* Enjoy structured chaos.

## Formulas
####Sphere formula:
_sin( ( vertex_index + x ) &lowast; frequency + phase  ) &lowast; amplitude + center_.
* It changes each vertex one-by-one, ordered by one of the specified axes.
 * It's the vertex_index variable that gives it the flowing/chaotic motion.

####Background formula:
 _sin(x &lowast; frequency + phase) * amplitude + center_
* The background's made up of three colors: Red, Blue, and Green
* Each color has its own sine wave. This produces interesting results:
  * Give each the same frequency. Offset their phases by 120°. It'll loop through the rainbow.
  * Same frequency and same phase will have the sine waves line up to produce a greyscale.
  * What other patterns can you find? ***FIND OUT NEXT TIME ON WIREFRAME-BALL Z!!!!***
  * This [site](http://krazydad.com/tutorials/makecolors.php) explains what's happening here.

## Sliders


| Sphere Variables  | Description                                                               |
|-------------------|---------------------------------------------------------------------------|
| x/y/z_frequency   | Adjust how fast the sphere's vertices change on the respective axis.      |
| x/y/z_phase       | Adjust the phase of the sine wave. Keep each axis out of phase for chaos. |
| x/y/z_amplitude   | Adjust how much the sphere's vertices change on the respective axis.      |
| x/y/z_center      | Adjust the center of the sine wave. It offsets the sphere's position.     |
| which_order       | Affect the sphere's vertices in the order of the chosen axis.             |
| x/y/z_rotation    | Adjust how fast the sphere rotates on the given axis.                     |

| Background Variables  | Description                                                                                  |
|-----------------------|----------------------------------------------------------------------------------------------|
| r/g/b_frequency       | Adjust frequency of sine wave. Keep the same for rainbows. Different for more color variety. |
| r/g/b_phase           | Adjust phase of sine wave. Keep each 120° out of phase for rainbows. Closer for greyscale.   |
| r/g/b_amplitude       | Adjust range for the respective color. 255/2 covers every shade of the color.                |
| r/g/b_center          | Adjust what shades of color it fluctuates from. 25 covers dark shades, 200 for light, etc.   |

|   Misc Variables  | Description                                               |
|-------------------|-----------------------------------------------------------|
| count_increment   | Adjust how fast the background changes & sphere animates. |
| box_xrotate_speed | Adjust how fast the little box rotates on the x-axis.     |

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Goals in Life

* Add zoom support on smart phones.
* Allow camera controls similar to [OrbitControls](http://threejs.org/examples/misc_controls_orbit.html), with no restriction on zooming.
* Add in cool presets that I've discovered.
* Get the sphere to switch between black n white gradually.
 * Perhaps also make it difficult for the background to change _too_ drastically, so as not to incur epilepsy.
* Allow for customization of the formulas that affect the sphere vertices & background color.
 * Perhaps simply have several preset formulas to choose from? I want some tangent-within-sine functions in there!
* Acquire large sums of money.

## Credits

Couldn't have done this without my cat [Sekai](https://instagram.com/p/zqJ4ADRTvm/), the robust documentation of [Three.JS](http://threejs.org/docs/), and the simplicity of [Dat.GUI](http://workshop.chromeexperiments.com/examples/gui/).