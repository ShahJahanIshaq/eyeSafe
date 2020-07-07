# cautiousEye
cautiousEye is a drowsiness detector, mainly designed to support vehicle drivers, especially truck drivers, who mostly have to travel long distances. It uses computer vision techniques to calculate the identify important regions and sounds an alarm if it detects that the eyes are closed for too long. To set up:
## Installation of Libraries
You will need to have Python 3 installed along with pip. Run:

`pip install opencv-python`

`pip install scipy`<br>

`pip install imutils`<br>

`pip install numpy`<br>

`pip install playsound`<br>

Another library that has to be installed is **dlib**. The following link contains the tutorial to install dlib:<br>
https://medium.com/analytics-vidhya/how-to-install-dlib-library-for-python-in-windows-10-57348ba1117f<br>
## Prerequisites
Download the `shape_predictor.bat` file and the `alarm.wav` audio file given above.
## Running the code
Run `py cautiousEye.py -p {path to shape_predictor.bat} -a {path to .WAV alarm} -w {index of webcam}` to run the script.

If the alarm sounds even when the eyes are opened, try increasing the value of the constant **EYE_AR_THRESH** declared on **line 34**<br>
If the alarm does not sound even when the eyes are closed, increase the value of the constant **EYE_AR_THRESH** declared on **line 34**<br>
## Examples
`py cautiousEye.py -p Desktop\shape_predictor.bat -a Desktop\alarm.wav -w 0`
