# Eye_Movement_Painter

### Real-time Eye-animation system that can paint with eye movement.

#### This project originates from the [HCI course design repository](https://github.com/DuNGEOnmassster/HCI_Course_Design_playground/tree/main/Group2) as an independent project.

View our course reports [here](https://github.com/DuNGEOnmassster/HCI_Course_Design_playground/blob/dd4a830b6d9df7d4d12f346c083332f98e40b9b9/Group2/%E7%AC%AC%E4%BA%8C%E7%BB%84%E4%BA%BA%E6%9C%BA%E4%BA%A4%E4%BA%92%E5%A4%A7%E4%BD%9C%E4%B8%9A.docx)

The current research on eye movement mainly relies on binocular eye trackers, which include an infrared camera aligned with the pupil used to calculate the line of sight vector and a scene camera used to estimate the observation point of the line of sight in the scene.

![](./Readme_img/Sample.png)

However, this is not suitable for the home experimental environment. Therefore, we adopted a monocular line of sight estimation strategy based on facial landmarks and eyes keypoints. After tracking the eye and pupil points with the help of the pre-trained model, the coordinates were enlarged proportionally to the screen to achieve monocular line of sight estimation.

With opencv, we are able to

1. use eye movement to control mouse movement

![](./Readme_img/Tracking_basic.png)

In addition, with a painting program based on PyQT, we are able to 

2. use eye clicks to control mouse click in order to choose painting tools

![](./Readme_img/Tracking_click.png)

3. use mouth opening to control the start and end of painting.

![](./Readme_img/Tracking_paint.png)