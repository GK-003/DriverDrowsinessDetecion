# DriverDrowsinessDetecion
This program detects whether the driver is drowsy or not and alert the driver with text and speech ,if the driver is drowsy.

This Python program is a simple implementation of drowsiness detection system using computer vision and speech synthesis. The program uses the OpenCV library for computer vision and the Pyttsx3 library for speech synthesis.

The program starts by initializing the speech engine (Pyttsx3) and creating a video capture object (OpenCV) to capture video from the device's camera. Then, it creates a dlib face detector and face landmark predictor.

The program enters a while loop where it continuously captures video frames, converts them to grayscale, detects faces in the frames, and predicts 68 face landmarks for each detected face. The landmarks are used to define the eyes, and the aspect ratio of the eyes is calculated using the Detect_Eye function.

If the aspect ratio of the eyes is below a certain threshold (0.25 in this case), the program considers the person in the frame to be drowsy and displays "DROWSINESS DETECTED" and "Alert!!! WAKE UP DUDE" on the frame. Additionally, the program speaks out the "Alert!!! WAKE UP DUDE" text using the speech engine.

Finally, the program releases the video capture and closes all windows when the user presses the 't' key.
