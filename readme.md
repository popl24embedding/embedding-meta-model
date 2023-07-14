# Steps to use the embedding-based meta model:

## 1. Create Data Folder:
In the `data` directory, set up the following folders:
- `java_files`: This folder should contain a repository of Java projects. The structure should be `java_files/project/version`. The order and hierarchy of the files within this directory are not important. We will iterate over all the files and use only the `.java` files.
- `Project_Arff`: Place all the ARFF format files in this directory. These files are created based on a CSV file of features (instructions on creating them will be provided separately in section 2).
- `Results_Rest`: Save all the results of the different algorithms from the algorithm repository in this directory. Instructions on obtaining the results will be provided separately in section 2. This path uses the MATLAB algorithm repository.
- `MCW`: Save all the results of the MCW algorithm in this directory. Instructions on obtaining the results will be provided separately in section 2.

## 2. Extracting the Labels:
Please refer to the detailed readme file located in the `labels extraction` folder for instructions on extracting the labels.

## 3. Features Extraction:
- **Statistical Meta Features:** Execute the `statistical meta features.py` script to generate the statistical meta features.
- **Embedding-based Meta Features:** Please refer to the detailed readme file located in the `embedding java files` folder for instructions on extracting embedding-based meta features from Java files.

## 4. Run Meta Model:
Now that you have completed the necessary steps for the meta model, you can run the `meta-model.ipynb` notebook. The notebook is based on the `algo_pre_processing.py` file.

## General Comment:
Our data is divided into two batches. In the notebook, we use two directories and perform two readings of the features and labels. However, for your own data, you can choose to use only one directory. Instructions specific to your data are provided in detail in the `meta-model.ipynb` notebook, in section 4.



