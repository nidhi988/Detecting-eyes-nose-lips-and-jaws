# Detecting-eyes-nose-lips-and-jaws
Using opencv, dlib, python

extract face regions, including:

Mouth
Right eyebrow
Left eyebrow
Right eye
Left eye
Nose
Jaw

The facial landmark detector implemented inside dlib produces 68 (x, y)-coordinates that map to specific facial structures. These 68 point mappings were obtained by training a shape predictor on the labeled iBUG 300-W dataset.

The mouth can be accessed through points [48, 68].
The right eyebrow through points [17, 22].
The left eyebrow through points [22, 27].
The right eye using [36, 42].
The left eye with [42, 48].
The nose using [27, 35].
And the jaw via [0, 17].

we can use the following command to visualize the results:

#Detect eyes, nose, lips, and jaw with dlib, OpenCV, and Python
$ python detect_face_parts.py --shape-predictor shape_predictor_68_face_landmarks.dat 
	--image images/example_01.jpg
