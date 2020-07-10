## Contributors

1. Manan
2. Gaurav
3. Aditya

## Static Map Navigation:
-------------------------

- Mapping
   - Mapping can be achieved , using the ultrasonic sensors easily(thanks to the sensor modelling done!) , but accuracy is questionable!
   - I think the accuracy , will be enough for our purposes!

- Localisation
   - Here local localization is relatively simple 
   - Assuming that there is no drift in wheel odom , what we have to do is basically the position tracking by fusing IMU and odom
   - The main **problem** , how is going to localise itself in the map , beacuse that is easy with camera , as well as LIDAR , but very difficult to achieve with Ultasonic Sensors 

- Motion (Path Planning)
   - Relatively simple , when the robot is localised and we have a map of the surrounding
   - Direct ros package can be used (move_base)
   - Or we can code up our own planner(kinodynamic path planning!)
  
## Alternate Sensors:
----------------------

- Camera
   - If we use a monocular camera , then localisation will be simpler relatively

## To do:
---------

- Do more research on how localisation is done with Lidar and depth cams
   - Then think , how to implement it on Ultrasonic sensors
