# Drone-Landing-Site-Prediction
Drone Landing Site Prediction Using Computer Vision

This project is focused on developing a system that predicts optimal landing sites for drones using advanced computer vision techniques. The system leverages a combination of object detection, semantic segmentation, and optical flow analysis to generate an aggregated score heatmap. This heatmap is used to identify safe and viable landing zones for the drone.

Project Architecture:
Current Frame Processing:
The current video frame is fed into two models: an Obstacle Detection Model and a Segmentation Model.
Previous Frame Processing:
The previous frame is processed using an Optical Flow Model to capture motion information between consecutive frames.
Aggregated Score Heatmap:
The outputs from the Segmentation Model and Optical Flow Model are combined to generate an aggregated score heatmap, representing potential landing sites.
Final Landing Site Determination:
The aggregated score heatmap is then integrated with the output of the Obstacle Detection Model to finalize the predicted landing sites on the current frame.
This multi-step approach ensures that the selected landing sites are not only safe but also stable, taking into account obstacles, terrain segmentation, and motion dynamics.
