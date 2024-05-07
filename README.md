# dynamixal-pan-tilt-camera-cad
CAD files for the Dynamical Pan Tilt camera.

### Specification

|             |                                                                         |
|-------------|-------------------------------------------------------------------------|
| Mass        | 100 g (standard version) or 80 g (lite version)                         |
| Pan range   | ±90°                                                                    |
| Tilt range  | ±90°                                                                    |
| Camera      | Most Arducam USB cameras would work, or design your own camera housing  | 
| Software    | ROS Noetic package (see [below](#ros-code))                             |


### Demonstration video

https://github.com/AnthonyZJiang/dynamixel_pan_tilt/assets/8778250/a04f16a8-ec1d-4a47-b50e-7347ddd1794e

Note that the LED above the camera shown in the video is non-standard and excluded in the CAD model.

### Autodesk Fusion 360
The CAD model is also available in Autodesk Fusion 360. Click the image below to open the web view.

<a target="_black" href="https://a360.co/4aqoyKB"><img width="620" alt="image" src="https://github.com/AnthonyZJiang/dynamixal-pan-tilt-camera-cad/assets/8778250/9c16dcb3-a206-4d0d-94db-9c3fb3061820"></a>

### Part list

#### Standard version

| #  | Item                 | Description                         | Quantity | Acquisition |
|----|----------------------|-------------------------------------|----------|-------------|
| 1  | Dynamixel XL330-M288 | Smart servo                         | 2        | Purchase    |
| 2  | Arducam B0202        | 2MP wide angle low light USB camera | 1        | Purchase    |
| 3  | FPX330-H101          | Dynamixel frame for XL330           | 2        | Purchase    |
| 4  | FPX330-S102          | Dynamixel frame for XL330           | 2        | Purchase    |
| 5  | Base mount           | Base of the pan tilt device         | 1        | 3D print    |
| 6  | camera housing       | Housing for the camera              | 1        | 3D print    |
| 7  | Camera housing cover | Cover for the camera housing        | 1        | 3D print    |
| 8  | Lens cap             | Lens cap for Arducam UC-684         | 1        | 3D print    |
| 9  | DIN912 M2.5x20       | M2.5x20 socket head bolt            | 4        | Purchase    |
| 10 | DIN912 M2x5          | M2x5    socket head bolt            | 4        | Purchase    |
| 11 | Tappex 017M2.5       | M2.5 threaded insert                | 4        | Purchase    |
| 12 | Cable clip short     | Cable clip (optional)               | 4        | 3D print    |
| 13 | Cable clip long      | Long leg cable clip (optional)      | 1        | 3D print    |

#### Lite version

| #  | Item                 | Description                         | Quantity | Acquisition |
|----|----------------------|-------------------------------------|----------|-------------|
| 1  | Dynamixel XL330-M288 | Smart servo                         | 2        | Purchase    |
| 2  | Arducam B0202        | 2MP wide angle low light USB camera | 1        | Purchase    |
| 3  | FPX330-H101          | Dynamixel frame for XL330           | 2        | Purchase    |
| 4  | FPX330-S102          | Dynamixel frame for XL330           | 2        | Purchase    |
| 5  | Base mount lite      | Lightweight base                    | 1        | 3D print    |
| 6  | camera housing lite  | Lightweight camera housing          | 1        | 3D print    |
| 7  | DIN912 M2.5x20       | M2.5x20 socket head bolt            | 4        | Purchase    |
| 8  | DIN934 M2.5          | M2.5 hexigon nut                    | 4        | Purchase    |
| 9  | DIN912 M2x5          | M2x5    socket head bolt            | 4        | Purchase    |
| 10 | Cable clip short     | Cable clip (optional)               | 2        | 3D print    |
| 11 | Cable clip long      | Long leg cable clip (optional)      | 1        | 3D print    |

### ROS code
- Pan tilt device: https://github.com/AnthonyZJiang/dynamixel_pan_tilt_ros
- Camera: http://wiki.ros.org/usb_cam
