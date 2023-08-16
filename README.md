# ISEN613 Engineering Data Analysis - Course Project
This repository contains the required data and starter code reference for students enrolled in ISEN 613, Fall 2022

## Sample description
- **Sample1**: Laser power 250 W, Scan speed 10 Inches/min,	Powder flow rate 4 RPM (revolutions per minute)
- **Sample4**: Laser power 420 W, Scan speed 20 Inches/min,	Powder flow rate 4 RPM

## Description of Files and Folders
- **Ground_Truth_Sample1**: A folder that contains all the ground truth images for sample 1. The images have already been converted to B&W (Black & White)
- **Ground_Truth_Sample4**: A folder that contains all the ground truth images for sample 4. The images have NOT been converted to B&W and are raw images
- **Spectrogram_Tensors_Sample1.mat**: A MAT file that contains all the spectrograms associated with sample 1. Every spectrogram is named in the following format: Tensor_voxel_{index} and 129 x 15 x 6 which corresponds to 129 x 15 spectrograms for M1 P1 P2 M2 P3 P4 (M - Milling; P - Printing)
- **Spectrogram_Tensors_Sample4.mat**: A MAT file that contains all the spectrograms associated with sample 4. Every spectrogram is named in the following format: Tensor_voxel_{index} and 129 x 6 x 4 which corresponds to 129 x 6 spectrograms for P1 P2 P3 P4 (M - Milling; P - Printing)
- **Tensor_data_72_voxels.zip**: A zip file that contains 72 .mat files pertaining to spectrogram data of 72 voxels of sample 1. Each .mat file is a tensor of dimension 129x15x6. These 72 tensors were the input used in the CNN code. Change the directory name to your folder that contains the 72 .mat files and use the for loop to read them.
- **Tensor_data_90_voxels_sample4.zip**: A zip file that contains 90 .mat files pertaining to spectrogram data of 90 voxels of sample 4. Each .mat file is a tensor of dimension 129x6x4. Change the directory name to your folder that contains the 90 .mat files and use the for loop to read them. NOTE: The python code was developed to work with Sample 1. Please update the dimensions at all instances wherever required to be compatible with that of Sample 4.
- **Ground Truth - Voxel Tensor Index_ Sample1.xlsx**: An excel file that assists in associating the Ground_Truth images and Spectrogram_Tensors spectrograms. This remains consistent for both the samples except for columns C-F which correspond to sample 1 only
- **CNN_Implementation_Code.ipynb**: A starter jupyter notebook to read the data and a CNN implementation. The students are expected to modify the code to meet their project objective

## Note
- This is a research restricted data and we ask you to restrain from sharing this data outside of your project group
- If you require access to the raw data, please get in touch with the TA and we will upload it to the repository
