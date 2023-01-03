# Eye_Movement_Painter
Real-time Eye-animation system that can paint with eye movement.

The current research on eye movement mainly relies on binocular eye trackers, that is, an infrared camera aligned with the pupil is used to calculate the line of sight vector, and a scene camera is used to estimate the observation point of the line of sight in the scene, which is not suitable for the home experimental environment. unfriendly.
Therefore, we adopted a monocular line of sight estimation strategy based on facial landmarks and eyes keypoints. After tracking the eye and pupil points with the help of the pre-trained model, the coordinates were enlarged proportionally to the screen to achieve monocular line of sight estimation.

In addition, we a painting program based on PyQT, which realized eye movement control mouse movement and single-click selection of drawing tools based on monocular line of sight estimation; at the same time, in order to avoid the eye movement control function being too complicated, we introduced the detection and detection of keypoints in the mouth. Calculate and realize the opening and closing control of the mouth to start drawing/stop drawing.