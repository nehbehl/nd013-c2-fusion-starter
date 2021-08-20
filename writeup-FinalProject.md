# Writeup: Track 3D-Objects Over Time

Please use this starter template to answer the following questions:

### 1. Write a short recap of the four tracking steps and what you implemented there (filter, track management, association, camera fusion). Which results did you achieve? Which part of the project was most difficult for you to complete, and why?

Firstly, I implemented EKF to track a single real-world target with lidar measurement input over time and the RMSE plot shows a mean RMSE of smaller than 0.35.

In the second step, I implemented the track management to initialize and delete tracks, set a track state and a track score. 

Third step was  about implementing a single nearest neighbor data association to associate measurements to tracks.

Last step was to implement the nonlinear camera measurement model and fuse lidar and camera sensor information.


I found first step easier as compared to rest of the steps and the final step was bit confusing for me.
### 2. Do you see any benefits in camera-lidar fusion compared to lidar-only tracking (in theory and in your concrete results)? 
Yes, camera-lidar fusion provided more data to track better.

### 3. Which challenges will a sensor fusion system face in real-life scenarios? Did you see any of these challenges in the project?
In real life, there will be lot more track management required and uncertainity is highly increased. This project covers mostly ideal scenarios.

### 4. Can you think of ways to improve your tracking results in the future?
I believe tracking results can be improved more by more careful handling of possible scenarios.
