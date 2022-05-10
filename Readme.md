# Background removal
In this project I am going to learn how to change background using OpenCV Python. 

## Features
* Can change background in real-time
* Can be used in Zoom, Teams and other

## How to install
1. Clone this repository on your computer
`https://github.com/paveldat/background_removal.git`
2. Install all the requirements
`run libraries.bat` or
`pip install -r requirements.txt`
3. Run the program
`python main.py`

## Help
You might face issue with webcam not showing and you get errors.
To solve it just change the value in this line (for example to `1`).
`cap = cv2.VideoCapture(0)`
Increment this number until you see your webcam.

## Background
All background images could be found in img folder. 
Each image must be 640*480 pixels.

You can change this parametres here:
```
cap.set(3, 640)
cap.set(4, 480)
```
And after that you can upload images for the background of other sizes indicated in these two lines.

## Change background images
You can change background pressing "a" or "d". For exiting the program just press "q".

## Result
![Alt Text](https://github.com/paveldat/background_removal/blob/main/result/result.gif)

## Deleting the main video
You can also remove the original video by changing the following lines:
```
#imgStacked = cvzone.stackImages([img, imgOut], 2, 1)
#_, imgStacked = fpsReader.update(imgStacked, color=(255, 0, 255))
```
```
cv2.imshow("Image", imgOut)
```

## Result
![Alt Text](https://github.com/paveldat/background_removal/blob/main/result/result2.gif)