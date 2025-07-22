# Indoor-Object-Recognition-from-Point-Cloud-Data
This repository is part of a funded research project at Arizona State University focused on indoor object detection to support facility management tasks. The project utilizes 3D point cloud data collected using the Matterport Pro 3D scanner which collected both RGB and 3D data.
In the first phase of the project, the goal was to detect and classify commonly used chair models within the scanned indoor environments. Each chair instance in the point cloud data was manually segmented and labeled in CloudCompare software according to its specific model, as identified by the manufacturer.
To enhance the data quality, a noise reduction step was applied using MATLAB’s pcdenoise function. The effectiveness of this step is illustrated in the sample image provided below, which shows significant noise removal.


Subsequent data preprocessing and model development were performed in Python. Preprocessing steps included shuffling, rotating, and jittering the point cloud data to improve model robustness. The classification model was built using the PointNet architecture, a deep learning framework specifically designed for 3D point cloud analysis. Please see the following figure for the model architecture.  

The initial implementation of the model achieved a test accuracy of 67.05%. Ongoing work is focused on enhancing both the dataset and the model architecture to improve performance.

Paper to PointNet model: Qi, Charles R., et al. "Pointnet: Deep learning on point sets for 3d classification and segmentation." Proceedings of the IEEE conference on computer vision and pattern recognition. 2017.
