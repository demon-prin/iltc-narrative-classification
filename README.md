# iltc-narrative-classification
iltc-narrative-classification

# Project Overview  

This project is designed to process and classify narrative structures using deep learning techniques for Semeval2025 task 10-2. The main file to run is **begin25.ipynb**, which has been tested on Python 3.12.6 and requires Jupyter Notebook with a Python kernel. You can modify the variables within this file to customize the model according to your requirements. The project has been tested only on Windows 11.

## Dataset Structure  

The raw dataset file (in English), containing every sentence, must be placed in the following directory:  
```dataset/raw-documents``` from the root of the project.
Additionally, you need to define the following three files within the `dataset` folder:

1. **dataset/dev.txt**  
   - This file contains the dataset predictions to be sent to SemEval.  
   - Each line should include a filename, and each line must be terminated with a newline character (`\n`).  

2. **dataset/test.txt**  
   - This file is used to calculate metrics like validation and threshold determination, which will later be applied to the `dev.txt` dataset.  

3. **dataset/train.txt**  
   - This file is used to define the training dataset.  

There are present few created samples to help the setup of files in those folders.

### File Format  
Both `test.txt` and `train.txt` must follow the SemEval2025 file convention:  
```
File.txt/tNarrative/tSubnarrative/n
```
### Libraries needed
You need to install the following libraries:
```
tensorflow
keras
numpy
json
pickle
torch
matplotlib
transformers
```

### Old Model
Through, uncommented and not reviewed,in ```2024``` folder its present the version of the model used for 2024 post task(after the end of the competition) 4-2a and 2b, as can be seen the 2025 model its an edit of post task 2024 model.