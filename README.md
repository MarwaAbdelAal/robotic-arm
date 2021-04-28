## This program shows how to composite modeling transformations to draw translated and rotated hierarchical models Using OpenGL.

### **1-Apply transformations to animate the model:**
   * Fixed point rotation is applied on the whole arm.
   * I faced a little problem in the rotation of fingers, first i was rotating all of them in the same direction but it showed up that i should rotate the other fingers in opposite direction of the thumb. So, i handled it by changing the sign of the rotating angle to inverse the rotating matrix. 

Before | After
  -----|------
  <img src="./images/before.png" alt="Before" title="Before" width="100%" height="220" /> | <img src="./images/after.png" alt="After" title="After" width="100%" height="220" />

#

### **2-Interaction with keyboard:**

* pressing the 's' and 'S' keys alters the rotation of the shoulder in and out respectively. Its limitations from -90 to 90 degress.
Shoulder In | Shoulder Out
  ----------|-----------
  <img src="./images/shoulder_in.png" alt="Shoulder In" title="Shoulder In" width="100%" height="220" /> | <img src="./images/shoulder_out.png" alt="Shoulder Out" title="Shoulder Out" width="100%" height="220" />

* pressing the 'e' and 'E' keys alters the rotation of the elbow in and out respectively. Its limitations from 0 to 130 degress.
Elbow In | Elbow Out
  -------|---------
  <img src="./images/elbow_in.png" alt="Elbow In" title="Elbow In" width="100%" height="220" /> | <img src="./images/elbow_out.png" alt="Elbow Out" title="Elbow Out" width="100%" height="220" />

* pressing the 'f' and 'F' keys alters the rotation of the fingers bases in and out respectively. Its limitations from 0 to 90 degress.
  
* pressing the 'g' and 'G' keys alters the rotation of the fingers ups in and out respectively. Its limitations from 0 to 130 degress.

Fingers Bases In | Fingers Ups In
  ---------------|---------------
  <img src="./images/fingers_in.png" alt="Fingers Bases In" title="Fingers Bases In" width="100%" height="220" /> | <img src="./images/fingerUps_in.png" alt="Fingers Ups In" title="Fingers Ups In" width="100%" height="220" />


## Requirements

```
sudo apt-get install freeglut3-dev
```

### then run project on windows or compile in linux By:

```
gcc -o arm arm.c -lGL -lGLU -lglut -lm
./arm
```