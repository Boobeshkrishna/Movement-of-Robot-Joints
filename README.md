# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
# DEVELOPED BY : BOOBESH PM
# REG NO : 212222233001
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)
```
## Output
### 1. Generic Articulated Robot
![image](https://github.com/Boobeshkrishna/Movement-of-Robot-Joints/assets/141472052/9019fc3a-5fb1-42bb-9157-a6e609e474e3)

### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/Boobeshkrishna/Movement-of-Robot-Joints/assets/141472052/e4b98f4c-0b71-491e-9492-95f6d63f3919)

### 3. Movement of Joint1
![image](https://github.com/Boobeshkrishna/Movement-of-Robot-Joints/assets/141472052/db301dea-df55-49fa-8063-6061889841ad)

### 3. Movement of Joint2
![image](https://github.com/Boobeshkrishna/Movement-of-Robot-Joints/assets/141472052/fd5cede3-af31-4f1e-8209-c0edbafb29fd)

### 3. Movement of Joint3
![image](https://github.com/Boobeshkrishna/Movement-of-Robot-Joints/assets/141472052/56ccab0f-0071-4d32-b262-38b25a48ff16)

## Result 
Thus the different robots joints are moved with the help of python list.


