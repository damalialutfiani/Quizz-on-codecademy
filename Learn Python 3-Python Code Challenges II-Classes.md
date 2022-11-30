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

4.  Controlling Them All

    We want to add a new feature which allows the use to control multiple robots at once. The robots should be able to all have the same latitude and longitude GPS destination coordinates as well as a setting for disabling them all called all_disabled. We can accomplish this using class variables. Here is how we can do it:

        a.  Create a new class variable within the DriveBot class called all_disabled and set it equal to False
        b.  Create a new class variable within the DriveBot class called latitude and set it equal to -999999
        c.  Create a new class variable within the DriveBot class called longitude and set it equal to -999999
        d.  Outside of the class, test the class variables by setting the longitude of all robots to 50.0, the latitude to -50.0 and all_disabled to True

    >   Coding question

        Create a class variable called all_disabled which is set to False. Next, create two more class variables called latitude and longitude. Set both of those variables to equal -999999. A third robot has been created below the first two robots. Set the latitude of all of the robots to -50.0 at once. Additionally, set the longitude of the robots to 50.0 and set all_disabled to True. You should be able to set those values using three lines of code.

    >   Code    :

        class DriveBot:
          # Create the class variables!
          all_disabled = False
          latitude = -999999
          longitude = -999999

          def __init__(self, motor_speed = 0, direction = 180, sensor_range = 10):
                self.motor_speed = motor_speed
                self.direction = direction
                self.sensor_range = sensor_range
    
          def control_bot(self, new_speed, new_direction):
                self.motor_speed = new_speed
                self.direction = new_direction

          def adjust_sensor(self, new_sensor_range):
                self.sensor_range = new_sensor_range

        robot_1 = DriveBot()
        robot_1.motor_speed = 5
        robot_1.direction = 90
        robot_1.sensor_range = 10

        robot_2 = DriveBot(35, 75, 25)
        robot_3 = DriveBot(20, 60, 10)

        # Change the latitude, longitude, and all_disabled values for all three robots using only three lines of code!
        DriveBot.longitude = 50
        DriveBot.latitude = -50
        DriveBot.all_disabled = True

        print(robot_1.latitude)
        print(robot_2.longitude)
        print(robot_3.all_disabled)

    >   Result  :

    ![python II - 5 4](https://user-images.githubusercontent.com/74751990/204672987-191b59be-6597-4468-b6bd-a7c94cb893c2.jpg)

5.  Identifying Robots

    In order to keep track of the robots we are creating, we want to be able to assign an ID value to each robot when it is created. If we create five robots in a row, we want the IDs of each robot to be 1, 2, 3, 4, and 5 respectively. This can be accomplished by using a class variable counter which increments and is assigned to an instance variable for the ID whenever the constructor is called. Here are the steps:

        a.  Create a new class variable in the DriveBot class called robot_count
        b.  In the constructor, increment the robot_count by 1
        c.  After incrementing the value, assign the value of robot_count to a new instance variable called id.


    >   Coding question

        Within the DriveBot class, create an instance variable called id which will be assigned to the robot when the object is created. Every time a robot is created, increment a counter (stored as a class variable) so that the next robot will have a different id. For example, if three robots were created: first_robot, next_robot, and last_robot; first_robot will have an id of 1 next_robot will have an id of 2 and last_robot will have an id of 3.

    >   Code    :

        class DriveBot:
          # Create a counter to keep track of how many robots were created
            all_disabled = False
            latitude = -999999
            longitude = -999999
            robot_count = 0
 
           def __init__(self, motor_speed = 0, direction = 180, sensor_range = 10):
                self.motor_speed = motor_speed
                self.direction = direction
                self.sensor_range = sensor_range
                DriveBot.robot_count += 1
                self.id = DriveBot.robot_count
                # Assign an `id` to the robot when it is constructed by incrementing the counter and assigning the value to `id`
    
            def control_bot(self, new_speed, new_direction):
                self.motor_speed = new_speed
                self.direction = new_direction
 
            def adjust_sensor(self, new_sensor_range):
                self.sensor_range = new_sensor_range

        robot_1 = DriveBot()
        robot_1.motor_speed = 5
        robot_1.direction = 90
        robot_1.sensor_range = 10

        robot_2 = DriveBot(35, 75, 25)
        robot_3 = DriveBot(20, 60, 10)

        print(robot_1.id)
        print(robot_2.id)
        print(robot_3.id)

    >   Result  :

    ![python II - 5 5](https://user-images.githubusercontent.com/74751990/204921567-68479d12-c8e2-4c61-9370-71945d03f538.jpg)
