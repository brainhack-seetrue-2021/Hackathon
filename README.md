# DSTA Brainhack SeeTrue 2021 Hackathon  


<p align="center">
  <img src="https://www.dsta.gov.sg/images/default-source/brainhack/seetrue-workshop-logo.png" />
</p>  


Welcome to the official code repository of the DSTA Brainhack SeeTrue 2021 Hackathon!

## Getting started

The repository contains a [Jupyter](https://jupyter.org/) notebook which provides a sample implementation of deepfake detection via a [InceptionV3](https://arxiv.org/abs/1512.00567) model. The notebook serves as a quick start for the hackathon! You can choose to build upon this model or even better, build one entirely by yourself!

We strongly encouraged you to use [Google Colaboratory]("https://research.google.com/colaboratory/") for the hackathon! Google Colaboratory is an online browser-based platform that allows us to train our models on Google Cloud virtual machines(yes with GPUs!) for free! Check out this [Youtube video](https://www.youtube.com/watch?v=inN8seMm7UI) to get up to speed quickly with Google Colaboratory! 

To get started, open the notebook in Google Colaboratory:

[![Open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1HoZog2DuloPXC9X83aGtcHA-sfX8g8Us)

## Dataset

For this hackathon, you will need to use the dataset that is provided. Please note that usage of external dataset is strictly not allowed in this hackathon!

The dataset can be downloaded via this [link](https://bit.ly/3w0xyBl).

The dataset is given in 2 formats: 
1) Raw video – Participants process video themselves
2) Extracted face from video frames - a group of images with facial features extracted from the given video


Directory structure of dataset:

<p align="center">
  <img src="https://i.ibb.co/cktRD8g/directory.png" />
</p>

## Submission of results

Participants are required to submit their model inference results in the format of a CSV file.

The CSV file should contain the prediction probability per video (i.e. participants using extracted dataset to aggregate score on the group of images of a video)
0 = fake, 1 = real. Participants to submit probability score (0..1), not binary score.
Please submit in order of video filename (i.e. 00000 to 00789), with header.

e.g. of CSV file:

<p align="center">
  <img src="https://i.ibb.co/zFtRmjB/See-True-Hackathon-Admin-Brief.png" />
</p>

In the provided Jupyter notebook, we have provided a helper function to generate the CSV file. You can use it directly if your model produced the same output as the demo model.

<p align="center">
  <img src="https://i.ibb.co/4SpsfBP/save-csv.png" width="600" height="800"/>
</p>

The CSV file and the corresponding Jupyter notebook can then be submitted for scoring via this [link](https://forms.gle/WjdkMUkfZce4hsNy5).

You can check for your submission status and score via the results portal: https://competition.azurewebsites.net/api/score?email={email}
NOTE: Please replace the placeholder {email} with the email you use during the submission of results.   
Example: https://competition.azurewebsites.net/api/score?email=abc123@gmail.com  
  
<p align="center">
  <img src="https://i.ibb.co/CW84RC9/See-True-Hackathon-Admin-Brief.png"/>
</p>

Please refer to the timestamp for the time of submission and the corresponding score of that submission. The submission that is not scored yet but is successfully received will be shown as "Pending" on the Score column. Please be patient and check back again for the updated score if your score is not reflected. Do approach your mentor for help if the score is not showing after an extended period of time.


