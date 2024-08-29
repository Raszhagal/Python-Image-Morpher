<p align="center">
  <img src="https://i.imgur.com/SLDEtSR.png"><br>
</p>

Python Image Morpher (PIM) is a program that can take two images and blend them to whatever extent or precision that you like!
It is designed to emulate some of Python's OpenCV image processing from scratch without reference.

<p align="center">
  <img src="https://media3.giphy.com/media/ibAOyLgNhxnWHuKvZn/giphy.gif"><br>
</p>

This project began in Spring 2019,
requiring the usage of <b>delaunay triangulation</b>, <b>projective/affine transformation</b>, <b>application of projections 
through matrices</b>, <b>masking,</b> and <b>alpha blending</b> - all of which are still maintained - in order to accomplish image 
morphing. Thus, this repository is more of a 'proof of concept' than it is the most efficient way of accomplishing the given task of image morphing. 

So far, this program has only been tested on separate Windows environments; 
if it does not already, later releases are likely to support Mac and Linux.

<p align="center">
  <img width="846" height="795" src="https://i.imgur.com/E8heqDa.png"><br>
</p>

## Installation:
This program has dependencies that do not come packaged with Python 3. To install the required modules, enter the following command using the terminal supplied by Windows or your choice of IDE (such as PyCharm):

```pip install -r requirements.txt```

Alternatively, for each module below that your machine does not have installed, enter the respective command(s):

<b>[PyQt5](https://pypi.org/project/PyQt5/)</b> - ```pip install pyqt5```

<b>[SciPy](https://pypi.org/project/scipy/)</b> - ```pip install scipy```

<b>[NumPy](https://pypi.org/project/numpy/)</b> - ```pip install numpy```

<b>[Imageio](https://pypi.org/project/imageio/)</b> - ```pip install imageio```

<b>[Pynput](https://pypi.org/project/pynput/)</b> - ```pip install pynput```

<b>[OpenCV (Headless)](https://pypi.org/project/opencv-python-headless/)</b> - ```pip install opencv-python-headless```

<b>[Requests](https://pypi.org/project/requests/)</b> - ```pip install requests```

If pip, for whatever reason, is not installed on your machine, enter the following line in a terminal:
```
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
```
Followed by this line afterward:
```
python get-pip.py
```

## Usage:
- Run MorphingApp.py either through the terminal or using an IDE
- Use the graphical interface to select the two images you want to morph together
- Alternate clicking on related points of interest in your images to create correspondences
- When satisfied, click the blend button to observe the result!

A more detailed Help guide is included within PIM's GUI, if needed.

<p align="center">
  <img src="https://i.imgur.com/ymCNhwS.gif"><br>
</p>
<p align="center"><i>Proof of Concept - Perspective Shifting</i><p align="center">

## Development 'To-Do' List:
Although I feel that PIM is now feature complete as a project, I will continue to support it with updates as they come to me. This potentially includes, but does <b>not</b> guarantee:
- <b>Feature:</b> Automatic Correspondence Determination
    - PIM may automatically generate points by scanning for similar features between images
- <b>Feature:</b> Automatic Update Installation
- <b>Enhancement:</b> Undo/Redo Compatibility with Move/Delete Mouse Modes

If you encounter an error, a bug, or if you simply wish to request a change/feature, please file an issue using the tracker that GitHub provides [here](https://github.com/Raszhagal/Python-Image-Morpher/issues).