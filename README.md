# LSC50-Colombian-Sign-Lenguage-Video-and-Inertial-Measurent-Dataset

The LSC50: Colombian Sign Language Video Dataset database explores the specific case of the recognition of 50 signs defined in Colombian sign language. The database has 4000 videos distributed in RGB, depth, and IR. Additionally, it has inertial measurement information involved in the movement of each of the signs. Moreover, finally, landmark files associated with the RGB videos were obtained. The total information in the database is equally distributed in the number of classes (50 signs) and the number of participants involved (5 volunteers: 3 native speakers and two non-native speakers).

We provide scripts to load and read our database made up of videos and Excel files, the .mot or .sto files must be read using OpenSim. The script was coded using Python 3.7.9. All scripts were tested on Windows. 

To use the data from inertial sensors in OpenSim, the data available in the RAW folder must be prepared. This data contains information related to the motion such as orientation and acceleration that are required to import the data to OpenSense, the OpenSim package for using inertial sensors. This package requires the .sto file included in the STO folder. It contains the orientation information obtained from the sensors, associated with each body segment. With these files, OpenSense places the sensors in each segment of the biomechanical model and allows the calculation of the inverse kinematics by generating the .mot file, which can be found in the OUT\_OPENSIM folder. These files contain kinematic data related to the motion required for the signs recorded.  This information was included in the “IMU” subsection of the “Data Records” section.  For more details, please see the guide available to OpenSim documentation: https://opensimconfluence.atlassian.net/wiki/spaces/OpenSim/pages/53084203/OpenSense+-+Kinematics+with+IMU+Data

The code is publicly available under the MIT OpenSource license. Therefore, permission is granted free of charge to copy and use this software and its associated files.


