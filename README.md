# TimeKit
A set of patches that keep time when Origami slows down. <br />
They behave mostly like standard Origami patches with the exception that Origami native patches seem to run at 60 FPS even though they have duration inputs in time. These versions run using device time so they are hopefully more accurate
<br />
Classic Animation+ <br />
Repeating Animation+ <br />
Stopwatch+ <br />
Repeating Pulse+ <br />
Cubic Bezier Animation+ <br />
Wait+ <br />
Delay 1x - this is an extension of Delay 1 but unlike Delay 1 it can delay for a number of frames greater than just 1. It is also loopable so you can delay for 0,1,2... frames and output a loop of delayed values <br />
<br />
I would love to be able to extend this to include a Delay+ patch, but this is a harder problem to solve because delay needs to record every value and then retrieve them at the appropriate time. The naturaly way to do this is with JSON, but once you start recording a lot of JSON Origami performance suffers noticably
