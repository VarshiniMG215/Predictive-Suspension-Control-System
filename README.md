# AI-Based Pothole Detection and Predictive Suspension Control System (Ongoing Project)

## Project Overview

This project focuses on developing an intelligent terrain monitoring and suspension response system for heavy-duty ** 6T DUMPER **mining trucks. The system aims to detect road irregularities such as potholes, ditches, bumps, and hard obstacles in real time before the vehicle reaches them. By combining LiDAR-based terrain sensing, sensor feedback, and machine learning analysis, the system predicts road disturbances and assists the suspension system in adapting accordingly to improve vehicle stability, safety, and ride comfort.

This is currently an **ongoing research and development project**, and the machine learning module for terrain classification and prediction is under active development.

## Objective

The main objective of this project is to build a predictive suspension control mechanism capable of detecting ground irregularities ahead of the vehicle and adjusting the suspension response before the vehicle encounters the disturbance.(ACTIVE SUSPENTION WE ARE USING)

Key goals include:

* Detect potholes, bumps, ditches, and obstacles on mining roads.
* Generate a real-time 3D terrain profile in front of the vehicle.
* Analyze ground height variations using sensor data.
* Provide predictive input to the suspension system to reduce vehicle shock and vibration.
* Improve safety and durability of heavy mining vehicles.


## System Architecture

The system integrates multiple sensing and control components to achieve predictive terrain monitoring.

### LiDAR Sensor

A 3D LiDAR sensorLIVOX Tele -15 is used to scan the terrain ahead of the vehicle and generate a point cloud representation of the ground surface. The LiDAR detects height variations that indicate potholes, bumps, or obstacles on the road.

### Processing Unit

An embedded AI computing platform processes the incoming LiDAR data and performs point cloud analysis. The processor extracts useful terrain features such as depth variations and surface irregularities.(nvidia jetson orin)

### Triaxial Accelerometer

A triaxial accelerometer  (MTN 2330) is installed on the vehicle chassis to measure real-time vibration and acceleration along the X, Y, and Z axes. This sensor helps monitor the vehicle's dynamic response when encountering road disturbances.

### Controller

An industrial controller (Beckhoff's)receives processed data from the computing unit and sensor inputs. The controller determines the required suspension adjustment based on detected terrain conditions.

### Active Suspension System

The suspension system adjusts its behavior based on the controller's commands by all ECU'S. By responding before the wheel reaches the irregular surface, the suspension system reduces shock transmission to the vehicle body.



## Working Principle

1. The LiDAR sensor scans the road surface ahead of the vehicle and generates a dense point cloud.
2. The processing unit analyzes the point cloud to identify depressions, bumps, or obstacles.
3. Terrain features are classified and distance to the irregularity is estimated.
4. The controller receives terrain information along with accelerometer feedback.
5. Based on prediction of the upcoming terrain disturbance, the suspension system prepares to absorb or adapt to the impact.
6. The vehicle passes over the irregularity with improved stability and reduced vibration.



## Key Technologies Used

* 3D LiDAR Terrain Sensing
* Point Cloud Processing
* Embedded AI Computing
* Sensor Fusion
* Triaxial Accelerometer Monitoring
* Industrial Controller-Based Actuation
* Predictive Suspension Control


## Machine Learning Component (Under Development)

The machine learning module aims to enhance terrain understanding by automatically identifying different types of road disturbances.

Planned ML capabilities include:

* Pothole detection
* Bump and hump classification
* Obstacle identification
* Terrain irregularity prediction

The ML model will be trained using LiDAR point cloud data and labeled terrain samples to improve detection accuracy.


## Challenges Addressed

During the development phase, several engineering challenges were analyzed and addressed:

* Selecting a suitable LiDAR sensor for mining environments.
* Understanding field-of-view limitations and blind zones.
* Calculating ground coverage area for tilted LiDAR mounting.
* Evaluating sensor performance in dusty and harsh environments.
* Integrating multiple sensors for reliable terrain detection.

---

## Current Project Status

This project is currently **in progress**.

Completed work:

* System concept design
* Sensor selection and evaluation
* Terrain coverage analysis
* Hardware architecture planning

Ongoing work:

* Machine learning model development
* Point cloud processing pipeline
* Sensor integration and real-time testing



## Future Scope

Future development will focus on improving prediction accuracy and system robustness through:

* Advanced machine learning models for terrain classification
* Real-time suspension actuation algorithms
* Integration with vehicle control systems
* Extensive field testing in mining environments



## Conclusion

This project aims to create a predictive terrain monitoring system that enhances the safety and performance of heavy-duty vehicles operating in harsh environments. By combining LiDAR sensing, real-time data processing, and machine learning, the system can anticipate road disturbances and assist the suspension system in responding proactively.

This is ongoing, and further development will focus on refining the AI-based detection models and implementing real-time hardware testing.
