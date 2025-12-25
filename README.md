Arduino Obstacle Avoiding Car

- An autonomous robot car that detects obstacles using an ultrasonic sensor and avoids them by changing direction using servo motor scanning and DC motor control.


 Features :
 1. Ultrasonic obstacle detection 
 2. Automatic forward & backward movement
 3. Servo-based left/right scanning
 4. Smart decision turning (chooses clear path)
 5. Uses Adafruit Motor Shield(AFMotor)


 Components Required :
 1. Arduino Uno 
 2. Adafruit Motor Shield
 3. 4 × DC Motors
 4. HC-SR04 Ultrasonic Sensor
 5. Servo Motor SG90 
 6. Robot Car Chassis
 7. Battery Pack (3.9V * 3 / 12V)
 8. Jumper Wires


Libraries Needed  :
Install the following libraries before uploading the code:

Library                 Source 
AFMotor       :         Required for Adafruit Motor Shield |
NewPing       :         Ultrasonic sensor handling |
Servo         :         Servo motor control |


 Installation Steps : 
1. Download library ZIP from the sources above
2. Open Arduino IDE → `Sketch`
3. Click `Include Library` → `Add .ZIP Library`
4. Select downloaded ZIP file and install
5. Repeat for all required libraries


Pin Configuration:

Sensor / Motor          Arduino Pin 
 TRIG                     A0 
 ECHO                     A1 
 Servo Signal             10 
 Motors                   Controlled via Motor Shield 



Working Logic : 
1. Car moves forward by default
2. If obstacle detected within 15 cm → STOP
3. Moves backward briefly
4. Servo scans left & right
5. Turns toward the side with more distance
6. Resumes forward movement


Code Upload : 
After installing libraries:
1. Connect Arduino
2. Select board & COM port
3. Click `Upload`

 
 Testing & Output : 
- Obstacle distance updates continuously
- Servo scans at 50° (Right) & 170° (Left)
- Car turns based on safest direction




