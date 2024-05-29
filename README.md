# LA3D Example
## Data
[LA3D](https://drive.google.com/file/d/1CnZ4_VOeoSilOU9MkITg_a7rgXMDtzXc/view?usp=sharing) 
## Label
The label files contain the following information. All values (numerical or strings) are separated via spaces, each row corresponds to one object. The 15 columns represent:

 Values |   Name   |   Description
--------|--------------|------------------------------------------------------
   1  |  type     |    Describes the type of object: 'Boat', 'Buoy'
   1  |  truncated |   Float from 0 (non-truncated) to 1 (truncated), where truncated refers to the object leaving image boundaries
   1  |  none  |   Ignored
   1  |  none    |    Ignored
   4   | bbox    |     2D bounding box of object in the image (0-based index): contains left, top, right, bottom pixel coordinates
   3  |  dimensions |  3D object dimensions: width, height, length (in meters)
   3  |  location  |   3D object location x,y,z in camera coordinates (in meters)
   1  |  rotation_z |  Rotation rz around Z-axis in camera coordinates [-pi..pi]

## Calib
The coordinates in the camera coordinate system can be projected in the image by using the 3x4 projection matrix P2 in the calib folder.

## Code
The code is realized based on [mmdetection3d](https://github.com/open-mmlab/mmdetection3d.git), coming soon!
