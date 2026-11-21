# Welcome to My Bouncing Box
***

## Task
/* What is the problem? */ 
The objective of this project is to replicate the classic Windows "Bounce" screensaver 
using vanilla JavaScript inside a pre-defined `index.html` file—without altering 
the existing HTML markup, using jQuery, or relying on `<canvas>`. 

/* where is the challenge? */
The challenge is to replace the box's text with my lowercase Qwasar login (`raustand_t`), 
animate it diagonally from `(0, 0)`, and accurately detect collisions with all four viewport borders 
so it reverses direction smoothly without getting stuck or triggering an infinite loop timeout.


## Description
/* How have you solved the problem? */
I solved this by selecting `#my_bouncing_box` via `document.getElementById` 
and updating its `textContent` to `"raustand_t"`. Using `setInterval`, 
the script increments the box's `x` and `y` coordinates on each tick and 
updates `style.left` and `style.top`. Before rendering each frame, it computes 
the maximum horizontal and vertical boundaries (`window.innerWidth - box.offsetWidth` 
and `window.innerHeight - box.offsetHeight`), clamps the position to the edge on contact, 
and inverts the corresponding velocity component (`vx` or `vy`) so the box bounces cleanly off every wall.

## Installation
/* How to install your project? npm install? make? make re?
No external dependencies or build steps are required. 
Clone the repository to your local machine:
```
git clone git@git.us.qwasar.io:my_bouncing_box_220942_p97mpc/my_bouncing_box.git
cd my_bouncing_box
```
## Usage
/* How does it work? */
Open index.html directly in any modern web browser (or launch the static HTML web previewer in Docode) to start the animation.

### The Core Team
TESSOH TCHINDA RAUSTAND (raustand_t)

<span><i>Made at <a href='https://qwasar.io'>Qwasar SV -- Software Engineering School</a></i></span>
<span><img alt='Qwasar SV -- Software Engineering School's Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px' /></span>
