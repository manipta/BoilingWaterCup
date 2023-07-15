Animation can be watched [here](https://www.instagram.com/reel/CqCVc5-NIFn/?utm_source=ig_web_copy_link)
Note:
required for assignment 1 is done:
	1. 1500 particles included
	2. force of gravity and friction is added
	3. collision handelling is done to kill particle at the top
	4. particles always remain in the scene
 	5. we are using blender for this
additional:
	1. aesthetic look
	2. camera is rotating
	3. steam is added(using volume)
as the project is a little longer i will tell some steps to the main functionalities/objective to the project. 
We're going to start off by making a little container and we're going to create some bubbles with some particles and create a displaced surface. 
hit A to select all x to delete

**making of cup
start off with a cylinder (shift+a cylinder). 
hit S to scale and let's grab Z bring it up so it's sitting on the ground 
go into edit mode, hit 3 on your keypad to go to face mode 
delete top and the bottom face 
hit Alt and select bottom loop 
hit E to extrude and S to scale 
hit F3 and type in grid fill. 
hit A to select all 
E to extrude 
S to scale then shift Z that turns off scaling on the Z axis(going to scale on the X and the Y)
bring a little thickness on cup 
switch to transparent mode, go into side view, hit B to box select and deselect top edges (do that with face mode)
hit G and Z and just bring it up until it got a nice thick bottom 
get out of transparent mode

**adding modifiers

come over to modifiers 
add in a bevel modifier 
adjust it to two segments 
add in a subdivision surface 
right click on cup shade smooth 

we got the cup. 

**to emit the bubbles and destroying them

***emitter

select the base, which is the perfect size we need because it fits just right in the bottom of the cup.
hit shift to duplicate. 
hit P (this will bring up the separate quick menu and select by selection. )
in edit mode, you can see two cylinders perfectly sized for the inside of cup. one is emitter other is surface. 
shift D to duplicate and then grab Z and bring this up 
it will be the surface of water. 
remove unrequired modifiers now

***in surface

add in a displacement modifier 
Click new for a new texture. 
Click button to the texture tab, 
give values to randomise it
create a little bit of variation and the height 
wrench tab (modifier property) adjust the strength.change the scale a little bit down. and the size.increase it.
create a few more subdivisions for displacement 
just increase to three on both the level viewport and the render
place the noise texture, the Voronoi noise texture. 
another object to use for the coordinates. 
click object then little drop down menu
create an empty object axis 
go back to the surface. And select empty 
wherever this empty goes, it's going to take that Voronoi noise pattern with it. 
click on the Z location of this empty 
type the #frame. ( it will take the current frame of our animation)

**particle system added

add a UV sphere. shade smooth.
come to our emitter. particle tab, the plus symbol to create a new particle system And right down ,to render. 
And change halo to render as object and select our sphere, which is going to be our bubble.
turn up the scale random ,increase the scale
one problem is if we play, bubbles are going in the wrong direction.
in particle system, gravity is set to one 
set that to -1,
problem solved

**kill particles going above

click the surface and go to the physics tab. And on the surface of water, turn on collision. 
here button called kill particles. Turn that on.
now this was the basic functionality you can add materials of your own and your innovation.

The tutorial or content like rotating camera and all can be explored on below link
https://youtu.be/1oD3gSX3ICM

Total Words : 667
