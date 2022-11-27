**Python Code Challenges II - Classes**

1.  Setting Up Our Robot
    Let’s begin by creating the class for our robot. We will begin by setting up the instance variables to keep track of important data related to the robot. Here are the steps we need to do:

        a.  Create a new class called DriveBot
        b.  Set up a basic constructor (no parameters needed)
        c.  Initialize three instance variables within our constructor which all default to 0: motor_speed, direction, and sensor_range

    >   Coding question

        Create a python class called DriveBot. Within this class, create instance variables for motor_speed, sensor_range, and direction. All of these should be initialized to 0 by default. After setting up the class, create an object from the class called robot_1. Set the motor_speed to 5, the direction to 90, and the sensor_range to 10. Use the provided print statements to check your work!

    >   Code    :

        # Define the DriveBot class here!
        class DriveBot:
            def __init__(self):
                self.motor_speed = 0
                self.direction = 0
                self.sensor_range = 0

        robot_1 = DriveBot()
        robot_1.motor_speed = 5
        robot_1.direction = 90
        robot_1.sensor_range = 10

        print(robot_1.motor_speed)
        print(robot_1.direction)
        print(robot_1.sensor_range)

    >   Result  :

    ![python II - 5 1](https://user-images.githubusercontent.com/74751990/204146996-c83b6b73-536f-451a-a571-c753eecfec40.jpg)

2.  Adding Robot Logic
    
    Now we want to add some logic to our robot. It would be very useful to be able to control our robot, so we are going to create a control_bot method which changes the speed and direction. We are also going to create a method called adjust_sensor. This method is used to change the range of our robot’s sensors which are used to detect obstacles. Here are the steps:

        a.  Define a function within the DriveBot class which accepts two additional parameters: one for a new speed and one for a new direction
        b.  Replace the instance variables for speed and direction with the input parameters
        c.  Define another function called adjust_sensor which accepts one additional parameter
        d.  Replace the instance variable sensor_range with the input parameter

    >   Coding question

        In the DriveBot class, add a method called control_bot which accepts parameters: new_speed and new_direction. These should replace the associated instance variables. Create another method called adjust_sensor which accepts a parameter called new_sensor_range which replaces the sensor_range instance variable. Afterwards, use these methods to rotate the robot 180 degrees at 10 miles per hour with a sensor range of 20 feet. Use the provided print statements to check your code!

    >   Code    :

        class DriveBot:
            def __init__(self):
                self.motor_speed = 0
                self.direction = 0
                self.sensor_range = 0
    
            # Add the methods here!
            def control_bot(self, new_speed, new_direction):
              self.motor_speed = new_speed
              self.direction = new_direction
 
            def adjust_sensor(self, new_sensor_range):
              self.sensor_range = new_sensor_range

        robot_1 = DriveBot()
        # Use the methods here!
        robot_1.direction = 180
        robot_1.motor_speed = 10
        robot_1.sensor_range = 20

        print(robot_1.motor_speed)
        print(robot_1.direction)
        print(robot_1.sensor_range)

    >   Result  :






