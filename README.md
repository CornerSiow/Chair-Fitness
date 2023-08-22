# Chair-Fitness-Activity
Distinghing Learned and Non-Learned Chair Fitness Activity using K-Means Activation Score


Total 10 Chair-Fitness Activities from 14 person.
<br/>(1) Leg Kicks, (2) Sit to Stand, (3) Shoulder Flexion, (4) Shoulder Abduction, (5) Chair Push Ups, (6) Shoulder Blade Squeeze, (7) Extended Leg Raises, (8) Seated Side Stretch, (9) Neck Turns, and (10) Seated Calf Raises.

Train: Person ID: 1,2,3,4,5,6,7,8<br/>
Validation: Person ID: 9,10,11<br/>
Test: Person ID: 12,13,14<br/>

We used MediaPipe extracted the 3D Pose from each of the frame.
<br/>The file named as : class_activity_person.pickle
<br/>Data Shape: Frames, Joints, XYZ

You can use pickle package to load the data.

# Code
1) Train with all classes (<a target="_blank" href="https://colab.research.google.com/drive/102Itf091GPzpxDVmYiPeGVmnc0iKVDYz?usp=sharing">Colab</a>).
2) Train with 6 classes and then distinghing non-learned classes
