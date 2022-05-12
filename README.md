# Odometry_subscriber
A  ROS Node that subscribes  and converts encder ticks to odometry  for a UGV. 

Tick data from wheel encoders helps us determine how much each wheel (both the left and right wheels) has rotated. Since we know the radius of each wheel, we can use the tick data and the wheel radius data to determine the distance traveled by each wheel.

Knowing the distance traveled by each wheel helps us determine where the robot is located in its environment relative to some starting location. This process is known as Odometry. 

The first time you were exposed to the word “Odometry” was likely when you began driving a car. Right behind your steering wheel is typically your odometer. The odometer of your car measures the distance traveled by the vehicle relative to some starting point where the car was first driven. Odometry in robotics works the same way.

The ROS Node .py in the src folder describes and illustrate how to subscribe to the encoder ticks of your UGV . on the arduino micro controller we will have a publishing code that publish the distance travelled by the encoder . Then a ROS Node subscribes to the encoder tick to know the location of the robot at a particular specific given time(Odometry).
