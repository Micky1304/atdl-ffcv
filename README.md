# To the structure of this repository:

In short, explanations are in the main notebooks per framework, the other project specific notebooks only contain used time measures.

Note that the structure here is not identical to the actual project folder, so paths may need to be updated.
Each time measurement is conducted in a separate jupyter notebook to reduce caching effects from previous iterations.
The notebooks are ordered by the project they are used for and contain the section number within the seminar thesis.

First, **SplitDataset.ipynb** is responsible to split the large satellite image into smaller parts and convert them into the beton format. Additionally, the dataset spanning 200 GB is created and transformed there.
All visualizations are created in **Visualizations.ipynb** and those used in the thesis are contrained in the folder **Visualizations**

The folder **Test and Validation**, contains the main notebooks for each framework. There, all the necessary functionality is implemented and explained which is copied into the specialized notebooks.

Notebooks for the comparison of CephFS and SSD storage can be found in the folder **3.3_SSD** as well as **3.5_CPU/1_Data_Loading**
The time taken for loading the 200 GB dataset can be found within the folder **3.4_Out_of_Memory**

The **3.5_CPU** project is consists of 9 notebooks, split into data loading, preprocessing and model training.
For the GPU project, the data loading times from the CPU are reused, with new preprocessing and model training notebooks for PyTorch and FFCV in **3.6_GPU**.
