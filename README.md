[![CI](https://github.com/pininduwk/Depth-Estimation-Using-DPT-Model/actions/workflows/blank.yml/badge.svg)](https://github.com/pininduwk/Depth-Estimation-Using-DPT-Model/actions/workflows/blank.yml)

# Real-time Depth Estimation on Drone Footage Using DPT Model

## Project Description
This project aims to estimate the depth of a video stream in real-time using the DPT (Deep Depth Prediction Transformer) model. The project takes a drone footage as input and outputs the corresponding depth map of the scene.

## Technologies Used
* Python
* OpenCV
* PyTorch
* Transformers

## Project Workflow
1. Load the input video file using OpenCV.
2. Set up the output video file with the same frame rate and size as the input file.
3. Load the DPT model and its image processor using the Transformers library.
4. Iterate through each frame of the input video.
5. Convert the OpenCV BGR image to a PIL RGB image.
6. Prepare the image for the model by passing it through the image processor.
7. Run the model on the image and get the predicted depth map.
8. Interpolate the predicted depth map to the original size of the image.
9. Convert the depth map to a numpy array and normalize it.
10. Write the output frame to the output video file.
11. Repeat steps 5-10 for all frames in the input video.
12. Release the input and output video files.

## Additional Features
* Display the input and output video streams side-by-side using OpenCV.

## Requirements
* Python 3.x
* PyTorch
* Transformers
* OpenCV
* Numpy
* PIL

## Future Improvements
* Implement object detection to generate depth maps only for specific objects in the scene.
* Improve the accuracy of the depth maps by fine-tuning the DPT model on a custom dataset.
* Implement real-time object tracking to track the depth of moving objects.

## Conclusion
This project demonstrates the use of the DPT model to estimate the depth of a video stream in real-time. The project can be extended to solve various real-world problems, such as obstacle detection and collision avoidance for drones and autonomous vehicles.
