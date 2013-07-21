# plumcube

**A compass mixin for creating 3D cubes of all shapes and sizes... as long as that shape is a cube.**

## Ex-ante

If you think that Boy Scouts use [Compass](http://compass-style.org/) and Girl Scouts have [SASS](http://sass-lang.com/), you might want to click those links first. Plumcube is a Compass extension, so you'll need both SASS and Compass in order to use it. Find your [compass](http://compass-style.org/install/), get [SASS](http://sass-lang.com/download.html)-y, and you'll be good to go.

Note that the plumcube plugin relies on the 'Bleeding Edge' version of SASS, because 3D CSS animation is the Internet of the future. If you are already a SASS-y individual, be sure to check your currently installed version (`sass -v`) and upgrade to the pre-release gem (3.3.0.alpha - get it with `gem install sass --pre`) if necessary.

## Get plumcube'n

### On the command line
Install the plumcube gem with `gem install plumcube`.

### In config.rb
Add `require 'plumcube'` to the top of your config.rb file, along with calls to any other compass plugins you may be including in your project. 

### In the HTML
Each face of your plumcube must be marked up as an unordered list, wrapped up in a few `<div>` elements to control the different 3D axes. The base markup for the cube is:

    <div class="your-cube">
        <div class="cube-z">
            <div class="cube-y">
                <ul class="cube-x">
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                </ul>
            </div>
        </div>
    </div>
    
Note that the `your-cube` class can have any name, but the `cube-z`, `cube-y`, and `cube-x` classes need to remain in place in order for your cube to render properly. You can also add any additional classes or unique identifiers to the list items, the unordered list, and/or the container elements.

### Stay tuned for the next installment, in which I actually attempt to sit down and focus for long enough to complete these instructions!
