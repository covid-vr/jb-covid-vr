# COVID-VR

The COVID-19 pandemic brought several challenges to health systems worldwide. Since most patients with COVID-19 have lung infections, a Computer Tomography (CT) of the chest was often used to identify COVID-19 infections, as well as other classes of pulmonary diseases. Deep-learning architectures surfaced to automatically identify classes of pulmonary diseases, using the slices of CTs as inputs to classification models. This work proposes COVID-VR, a novel approach for classifying pulmonary diseases based on volume rendering images of the lungs taken from different angles, thus providing a global view of the entire lung in each image. We compared our pro- posal against leading competing strategies with available solutions, using private data from partner hospitals and publicly available data. Results show that our approach suc- cessfully identifies pulmonary lesions and is competitive against slice-based methods.

```{figure} /_static/lecture_specific/index/pipeline.png
---
name: pipeline
scale: 50%
---

**Figure 1:** The pipeline of our proposed COVID-VR approach is divided into two stages. Stage 1 carries out data preparation to obtain the input images for model development, which is conducted in Stage 2. Data preparation involves the steps of image resizing by interpolation, lung segmentation, 3D volume rendering using pre-defined transfer functions, and snapshots generation for axial and coronal planes In Stage 2, DL models are trained for each plane to distinguish among the classes of interest and their outputs are combined to obtain a final patient-level classification.

```
