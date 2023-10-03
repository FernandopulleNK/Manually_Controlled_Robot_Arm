# Manually_Controlled_Robot_Arm

- This robot arm was developed as a group project with my colleagues: Hiruna, Upeksha, Ramitha, and myself. The idea for a robot arm was inspired by watching the IRON MAN movie. We created a prototype of our design, which is manually controlled by the user.
- Watch the video to see how our robot arm appears : https://youtube.com/shorts/kjj0btYZ9HY?feature=share
- Watch the video to see how our robot arm operated in EXMO 2023 : https://youtu.be/sI3S3pkTjw0
  
![IMG_1373-E](https://github.com/FernandopulleNK/Manually_Controlled_Robot_Arm/assets/128304706/3e7f41f6-7596-49e3-a98a-ec8f6ed99a48)
![IMG_1375-E](https://github.com/FernandopulleNK/Manually_Controlled_Robot_Arm/assets/128304706/42a48d28-ca37-44cc-a20c-ff64e54e1e99)


## Specification of the arm
- Six degree of freedom is achieved by using six joints in the arm.
- End effector is gripper which can pick and place an object.
- ESP32 cam module is used at end effecter to find the object 
- Arm can be controlled from any where else by using the feedback of the cam module which gives feedback to user’s device through the Wi-Fi.
-  There is controller panel with six control knobs.

## Components and Modules Used
### Motors 
We used 5 servo motors and 1 stepper motor for the six joints.
- SG90 servo - end effector(gripper).
- Two MG90S Metal Gear motors and – Connect the middle links 
- 40Kg High Speed servo Metal Gear motors -Connect the middle links
- Nema17 Stepper Motor – Base Joint
  ![268157945-0a6f9660-51f2-477b-8905-7bf659530700](https://github.com/FernandopulleNK/Manually_Controlled_Robot_Arm/assets/128304706/c2645d63-49df-4efb-ad3e-3093acb3a0f6)

### Power supply

We found that when all the motors are working, the motors are driven about 5A current, because all the motors are at stall toque expect stepper motor. Therefore 10A power supply was designed by me. Output voltage of power supply is 12V.
![IMG_0981](https://github.com/FernandopulleNK/Manually_Controlled_Robot_Arm/assets/128304706/5d166e78-894b-49c4-b9fa-01f7e33c61e6)


### Controlling Circuit 

Atmega328p was used as microcontroller. There six potential meters to control each motor separately. All the servo motors were controlled by PWM signals as usual. 

12V Output of the power supply is given to 5V buck convertor which powered microcontroller and some servo motors. 

We used ESP32 cam module which can be connected to any device through the Wi-Fi at end effector. The purpose of using a cam module was user can be controlled the arm by observing output of cam module. Because user can see what the end effector orientation and position is.

### Our team.

![IMG_0971](https://github.com/FernandopulleNK/Manually_Controlled_Robot_Arm/assets/128304706/28152062-8e5a-4a94-8ee0-1d52c3162036)
![IMG_0946](https://github.com/FernandopulleNK/Manually_Controlled_Robot_Arm/assets/128304706/af5889d6-cdfb-46dc-bcd5-261fac1804a5)
