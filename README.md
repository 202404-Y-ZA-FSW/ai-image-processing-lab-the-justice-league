## Overview

In this activity, you will explore the process of using Python to perform image processing on video data. Specifically, you will learn how to use OpenCV to capture video frames and apply a pre-trained model, `Salesforce/blip-image-captioning-base`, to generate descriptions for each frame. By the end of this activity, you will have a Python script that processes a video file frame by frame and outputs textual descriptions for each frame.

This activity is designed to give you hands-on experience with video processing and machine learning integration using open-source tools. The tools and libraries you will use include:

- **Python**: The primary programming language for this activity.
- **OpenCV**: An open-source computer vision library used for video and image processing.
- **Salesforce/blip-image-captioning-base model**: A pre-trained model for generating captions for images which can be found [here](https://huggingface.co/Salesforce/blip-image-captioning-base).

The end result of this activity will be a series of text descriptions corresponding to the individual frames extracted from a video.
This exercise will help solidify your understanding of integrating machine learning models with traditional image processing techniques, and you'll gain practical experience in handling video data programmatically.
## Instructions
We have provided you with a video that you will use in this activity. You can copy its link directly from Github with this [link](https://github.com/user-attachments/assets/d024a685-8740-4537-94f7-e05bd512bdd7)


1. **Environment Setup**:
   - Ensure that Python is installed on your local machine or is accessible via Google Colab.
   - Install necessary libraries, including OpenCV and Hugging Face's `transformers` library for model handling.
   - You may also need to install additional dependencies as required by the `Salesforce/blip-image-captioning-base` model.

2. **Video Input**:
   - Select a video file that you would like to process. The video should be in a common format (e.g., `.mp4`, `.avi`).
   - Load the video file into your Python environment using OpenCV.

3. **Frame Extraction**:
   - Use OpenCV to read the video and extract frames in a sequential manner.
   - Consider the frame rate of the video to determine how many frames you will extract per second. This will depend on your goals (e.g., extracting every frame or every nth frame).

4. **Image Captioning**:
   - For each frame extracted, pass the frame through the `Salesforce/blip-image-captioning-base` model to generate a caption.
   - Ensure that each caption is stored in a list or dictionary along with the corresponding frame number or timestamp.

## Tips
1. Start small, first make sure that you have a function that can accept a single picture and can normally process it and return the result.
2. OpenCV is a new tool to you, but it is easy once you understand it. Make sure you get the frames one by one.
3. The video we provided is 9 seconds long. You don't need to process the whole thing from the beginning. Process the first 3 seconds and once you are confident that you have the code ready try it out on the rest of the 9 seconds.
4. Once you have the above working separately. Join them together by passing each frame one-by-one to the model to describe them.
5. Now that you have them all, save in a dictionary the frames and the description.

## Retrospective
After finishing the activity above, in what way can we make this useful? How can we make it better?
