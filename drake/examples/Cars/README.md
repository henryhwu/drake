How to run the car simulation
=============================

 

Additional prerequisites
------------------------

 

Install pygame (e.g. with brew install pygame, or apt-get install pygame)

 

Set up your python path, e.g. with

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
export PYTHONPATH="/path/to/drake-distro/build/lib/python2.7/dist-packages:/path/to/drake-distro/build/lib/python2.7/site-packages:$PYTHONPATH" 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

e.g. for me it is

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
export PYTHONPATH="/Users/russt/drake-distro/build/lib/python2.7/dist-packages:/Users/russt/drake-distro/build/lib/python2.7/site-packages:$PYTHONPATH" 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

 

Running the simulator
---------------------

 

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
cd drake-distro/drake/examples/Cars
../../../build/bin/drake-visualizer &     
python SteeringCommandDriver.py &        
../../pod-build/bin/carSimLCM prius/prius.urdf
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

 

Make sure that the (very small) pygame window has focus, then use your arrow
keys to drive around.  If you have a joystick / steering wheel.. you can use
that, too (see SteeringCommandDriver.py for details).

 
