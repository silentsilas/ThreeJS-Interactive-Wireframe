# ThreeJS-Interactive-Wireframe
Trippy visuals are to be had with the help of sine functions, Dat.GUI, and Three.js.

## Instructions

* Go to the [Site](http://poeticode.github.io/ThreeJS-Interactive-Wireframe/) in a modern browser.
 * Should also work on smart phones.
* Zoom in and out with the mousewheel. Smart phones can't zoom currently.
* Click on the two small objects to toggle their wireframe.
* Adjust the sliders to animate the giant bumpy sphere in weird ways.
* Enjoy structured chaos.

## Sliders

| Variable          | Description                                                          |
|-------------------|----------------------------------------------------------------------|
| count_increment   | Adjust how fast the background changes & sphere animates.            |
| x/y/z_amplitude   | Adjust how much the sphere's vertices change on the respective axis. |
| frequency         | Adjust how fast the sphere's vertices change.                        |
| whichOrder        | Affect the sphere's vertices in the order of the chosen axis.        |
| x/y/z_rotation    | Adjust how fast the sphere rotates on the given axis.                |
| box_xrotate_speed | Adjust how fast the little box rotates on the x-axis.                |

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
* Allow for customization of the formulas that affect the sphere vertices & background color.
 * Perhaps simply have several preset formulas to choose from?
* Acquire large sums of money.

## Credits

Couldn't have done this without my cat [Sekai](https://instagram.com/p/zqJ4ADRTvm/), the robust documentation of [Three.JS](http://threejs.org/docs/), and the simplicity of [Dat.GUI](http://workshop.chromeexperiments.com/examples/gui/).

## License

Check the LICENSE file