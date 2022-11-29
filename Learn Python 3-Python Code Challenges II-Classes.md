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

    ![python II - 5 2](https://user-images.githubusercontent.com/74751990/204165089-86a16e62-26a2-4101-822a-679ea099aa88.jpg)

3.  Enhanced Constructor

    It can be tedious manually setting the values for each instance variable after we have created an object from the DriveBot class. We can enhance our constructor to automatically assign the values we provide to the instance variables. Instead of taking zero parameters, we are going to make the constructor take three parameters. Here is what we need to do:

        a.  Modify the constructor to take three parameters (in addition to self): one for motor_speed, one for direction, and one for sensor_range
        b.  For the first parameter, make the default value 0
        c.  For the second parameter, make the default value 180
        d.  For the third parameter, make the default value 10
        e.  Within the constructor, replace the instance variables with the variables from the input parameters

    >   Coding question

        Upgrade the constructor in the DriveBot class in order to accept three optional parameters. The constructor can accept motor_speed (which defaults to 0 if not provided), direction (which defaults to 180 if not provided, and sensor_range (which defaults to 10 if not provided). These parameters should replace the associated instance variables. Test out the upgraded constructor by initializing a new robot called robot_2 with a speed of 35, a direction of 75, and a sensor range of 25.

    >   Code    :

        class DriveBot:
          def __init__(self, motor_speed = 0, direction = 180, sensor_range = 10):
            self.motor_speed = motor_speed
            self.direction = direction
            self.sensor_range = sensor_range
            
            # Update this constructor!
            #def __init__(self):
            #    self.motor_speed = 0
            #    self.direction = 0
            #    self.sensor_range = 0
    
            def control_bot(self, new_speed, new_direction):
                self.motor_speed = new_speed
                self.direction = new_direction

            def adjust_sensor(self, new_sensor_range):
                self.sensor_range = new_sensor_range

        robot_1 = DriveBot()
        robot_1.motor_speed = 5
        robot_1.direction = 90
        robot_1.sensor_range = 10

        # Create robot_2 here!
        robot_2 = DriveBot(sensor_range = 25, motor_speed = 35, direction = 75) 

        #
        print(robot_2.motor_speed)
        print(robot_2.direction)
        print(robot_2.sensor_range)

    >   Result  :

    ![python II - 5 3](https://user-images.githubusercontent.com/74751990/204582204-49bab4ef-1b5f-4bac-9220-d5d0c4c7fe70.jpg)




