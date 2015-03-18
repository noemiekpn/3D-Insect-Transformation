##Description
This program is a simple implementation of a 3D insect model in OpenGL, applying the concepts of hierarchical models in Computer Graphics. The insect is composed of 14 pieces in the following hierarchy:

THORAX
	HEAD
	UPPER LEG RIGHT 1
		LOWER LEG RIGHT 1
	UPPER LEG RIGHT 2
		LOWER LEG RIGHT 2
	UPPER LEG RIGHT 3
		LOWER LEG RIGHT 3
	UPPER LEG LEFT 1
		LOWER LEG LEFT 1
	UPPER LEG LEFT 2
		LOWER LEG LEFT 2
	UPPER LEG LEFT 3
		LOWER LEG LEFT 3

Each of the pieces above can be transformed by rotating in the x, y and z-axis, when each case is possible. Restrictions on the angles for each axes were imposed for a more coherent movement. Joints in the forms of spheres where placed to present better connection between these pieces, as well as the eyes and antennae for better representation. These cannot be individually transformed.

This program also implements different view transformations, allowing the user to manipulate the position (pan), angle (rotate) and distance (zoom) of the view of the insect. The xyz-axes and a grid can be enabled for better understanding of direction and position.

##Interface controls
  ------------------------------------------------------------------
  	   **BUTTON**		      |		           **EFFECT**
	------------------------+-----------------------------------------
	'a'						          |	Show/hide xyz-axes
	'g'						          |	Show/hide grid
	'+'						          |	Zoom in 
	'-'					  	        |	Zoom out
	------------------------+-----------------------------------------
	's'					  	        |	Enable/disable piece selection
	Tab					         	  |	Select next piece
	Up-arrow				        |	Rotate clockwise around x-axis
	Down-arrow				      |	Rotate counter-clockwise around x-axis
	Left-arrow				      |	Rotate clockwise around y-axis
	Right-arrow				      |	Rotate counter-clockwise around y-axis
	Shift + Left-arrow		  |	Rotate clockwise around z-axis
	Shift + Right-arrow		  |	Rotate counter-clockwise around z-axis
	------------------------+-----------------------------------------
	Left-click				      |	Pan view
	Middle-click			      |	Rotate view
	------------------------+-----------------------------------------

##Sources
Most of this program was constructed upon the example code from Chapter 3 of the book "OpenGL Programming Guide: The Official Guide to Learning OpenGL" (7th Edition) by Dave Shreiner, Graham Sellers, John M. Kessenich and Bill M. Licea-Kane. Chapters 5 and 10 are supportive for hidden-surface removal concepts.

Online explanatory excerpts, reference and examples were observed from diverse websites such as Stack Overflow and Youtube tutorials and from:

https://www.opengl.org/
https://open.gl/depthstencils
http://www.zeuscmd.com/tutorials/
http://nccastaff.bournemouth.ac.uk/jmacey/RobTheBloke/www/
http://www.davidwparker.com/

##Author
Developed by Noemie Nakamura for the Computer Graphics course CSCE 441 at Texas A&M University in March 2015.

