# Email_webcam_thieft_detection_app_using_Python


**Project Description: Webcam-based Person Detection and Email Alert System**

This Python application utilizes OpenCV for real-time webcam monitoring to detect when a person enters the frame. Upon detection, it captures an image and sends an email alert with the captured image attached.

**Key Features:**
- **Real-time Monitoring:** Uses OpenCV to capture frames from the webcam and processes them for motion detection.
- **Motion Detection:** Compares consecutive frames to detect changes using image differencing techniques.
- **Object Detection:** Utilizes contour detection to identify areas of significant motion (i.e., people entering the frame).
- **Email Notification:** Sends an email notification using SMTP when a person is detected, attaching a snapshot of the moment.

**How It Works:**
1. **Frame Processing:** Captures frames from the webcam and converts them to grayscale for motion analysis.
2. **Motion Detection:** Computes the difference between the current frame and a reference frame to detect changes.
3. **Object Identification:** Identifies significant contours (areas with detected motion) using OpenCV's contour detection.
4. **Email Alert:** Initiates a separate thread to send an email with the captured image when motion is detected.
5. **Cleanup:** Periodically cleans up stored images to maintain system efficiency.

**Usage:** Ideal for applications requiring real-time monitoring and alerting, such as home security systems or occupancy monitoring in buildings.
