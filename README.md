# Project
This project is to distinghing Learned and Non-Learned Activity by using K-Means Activation Score.
<br/>
We first train a autoencoder model, and then used this encoder to generate the encoded features (Please find in the directory).
<br/>
Then, we generate a list of center nodes for each learned class by using k-means algorithm.
<br/>
Next, we obtains the activation score of each input data with the center nodes.
<br/>
Last, we fed the activation score features to a MLP model for final prediction. 


# Chair-Fitness Dataset
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
2) Train with 6 classes and then distinghing non-learned classes.



## Citing Us
If you find this project useful in your research, please use the following BibTeX entry for citation.
```BibTeX
@inproceedings{siow2023use,
  title={Use K-Means-Generated Nodes to Distinguish Learned From Non-Learned Exercises},
  author={Siow, ChyanZheng and Dou, WenBang and Song, QingWei and Chuquirachi, Franz and Obo, Takenori and Kubota, Naoyuki},
  booktitle={IECON 2023--49th Annual Conference of the IEEE Industrial Electronics Society},
  year={2023},
  organization={IEEE}
}
```


