# glviewportTest
 three center dots and plane with "center hole" using assymetric fov from hmd.  With glviewport verticalshift test. 
 
 Inputs: demo(verticalShift, drawPlane, drawCenterPoints, loadMVIdentity, holeSize, pointSize)
 
 verticalShift = 1 means set glViewport(0, 0, RectWidth(winRect), RectHeight(winRect) - vertical_shift).
 
 verticalShift = 0 means use "proper" viewport params i.e glViewport(0, 0, RectWidth(winRect), RectHeight(winRect))
 
 drawPlane = 1 means draw a plane with hole in the "center"
 
 drawPlane = 0 means do not draw plane
 
 drawCenterPoints = 1 means draw 3 opengl point primitives at pos(0,0 depths [-1,-2,-3])
 
 drawCenterPoints = 0 means do not draw center points
 
 loadMVIdentity = 1 means use identity for modelview, basically taking the camera and model transform out of the equation
 
 loadMVIdentity = 0 means use the modelview given by the oculus headset
 
 holeSize = size of the hole in the plane, if the plane is not drawn holeSize does nothing
 
pointSize = size of the centerPoints, if the points are not drawn then pointSize does nothing

These all have a default setting: demo(1,1,1,1,15,10) if nothing is passed to demo when ran.
