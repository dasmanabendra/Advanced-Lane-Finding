## Advanced Lane Finding Project

* Compute the camera calibration matrix and distortion coefficients given a set of chessboard images.
* Apply a distortion correction to raw images.
* Use color transforms, gradients, etc., to create a thresholded binary image.
* Apply a perspective transform to rectify binary image ("birds-eye view").
* Detect lane pixels and fit to find the lane boundary.
* Determine the curvature of the lane and vehicle position with respect to center.
* Warp the detected lane boundaries back onto the original image.
* Output visual display of the lane boundaries and numerical estimation of lane curvature and vehicle position.

### Discussion

* 
#### Challenges
* Tuning the threshold parameters was time consuming and therefore an automated method was implemented. 
* The pipeline did not perform well for the challenge and harder_challenge videos.
#### Improvement
* The criretion used to combine images obtained from color and gradient images could be modified to get better images under various light conditions.
* There are numerous parameters that are used at each stage of the pipeline. The optimization framework can be used to obtain better estiamtes for these parameters.   
* The threshold parameters could be made dynamic i.e. a different set can be changes based on the conditions.
#### Drwabacks
* The pipeline is not robust for every light conditions (e.g shadows) as evident from *challenge_video_out.mp4* and *harder_challenge_video_out.mp4*
* The pipeline won't perform well during lane changing.
