# Supplementary Material

Here, we summarize all the links to our repositories and results. Each repository contains an example of how to execute the contained source code.

## Full Pipeline
Our full pipeline presented and detailed in Chapter 5 with its requirements and examples of how to run are available in [[Full Pipeline link]](https://github.com/covid-vr/covid-vr-docker).

## Independent Repositories
In this Section we detail the main components of our Full Pipeline which can be used independently. Each repository contains an example of how to execute the code.

### Lung segmentation
Required packages and minimum versions. For complete detail see at require-
ments.txt in our adapted P-HNN version:
- Python 3.6
- Pytorch 1.3
- Cudatoolkit 10.1
- Anaconda

Link to repositories:
- Original P-HNN repository [[link]](https://adampharrison.gitlab.io/p-hnn/).
- Our adapted P-HNN version [[link]](https://github.com/covid-vr/p-hnn-lung-segmentation).
- Model Weights [[link]](https://drive.google.com/file/d/1l6yLFScULNw-oVoark0KZ-wnDFX8zwrN/view?usp=sharing).

### Visualization Repositories
Minimum required libraries:
- CMake 3.17
- QT 5.12
- MITK [[link]](https://github.com/MITK/MITK)
- ffmpeg (For video-generator repository)

Link to repositories:
- Repository to capture view images [[link]](https://github.com/covid-vr/camera-shots-generator).
- Repository for video generation from CT Image [[link]](https://github.com/covid-vr/video-generator).

Both repositories need as input an image in NIfTI format and a XML for the transfer functions, samples of both were added to each repository. We highly recommend using a Desktop environment (with UI); however, could be used in a server environment like our Full Pipeline, using VGLRUN command along with the steps described in Full Pipeline link.

### COVID-VR Proposed Network
Required minimum versions (the complete requirements are in the repository link):
- Python 3.6
- TensorFlow 2.0
Link to repositories:
- Repository for train and validation: [[link]](https://github.com/covid-vr/covid-vr-network).
- Model weights (For the two views) [[link]](https://drive.google.com/drive/folders/1OXTliIhm7yGuBDIL7qZhQrjCoaxmGx0l).

### Additional Resources
- Repository for get metrics (accuracy, precision, f1-measure, etc) and generate graphics used in this work [[link]](https://github.com/covid-vr/model-evaluation-metrics).
- Repository to generate Grad-CAM visualizations [[link]](https://github.com/covid-vr/covid-vr-grad-cam).
