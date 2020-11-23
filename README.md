# **Skin Cancer Detection**
# **Introduction**
Skin cancer is the most common cancer in the United States and worldwide. Over 5,400 people worldwide die of nonmelanoma skin cancer monthly and approximately more than $8.1 billion were spent every year for treating skin cancer in the U.S alone. The presence of preventative methods (like wearing sunscreen and sun protection, ...) might be largely helpful for the prevention of skin cancer. On the other hand, there have been ongoing attention focusing on the development of early detection of skin cancer based on pigmented lesions. This has become the motivation of this project.
# **Concept**
The development of Machine Learning (ML) and, especially, Deep Learning (DL) in Computer Vision has become the foundation of early detection of skin cancer using dermatoscopic images of unusual pigmented lesions from patients. Studying the potential patterns and similarity among these lesions can provide insightful information for early detection of potentially harmful skin cancer. 
This project emply the Skin Cancer MNIST: HAM10000 consisting of a large collection of multi-source dermatoscopic images of pigmented lesions from a wide range of patients (different populations, genders, ages, etc.). The dataset includes 10015 dermatoscopic images with the representation of 7 commnon types of pigmented lessions. Further information on the dataset can be found in the reference below.

# **Implementation**
The implementation of this project can be summarized as follow:
- Data exploratory
- The project consists of the TensorFlow implementations two approaches:
    + Image augementation with CNN
    + Transfer learning
- The dataset itself is largely imbalanced as specific diseases are more popular and frequently observed among patients than others. I, then, perform oversampling for those with limited train data and undersampling for those with larger train data to create the overall balance during training.
# **Performance**
- Image augmentation with CNN outperforms Transfer learning with the validation accuracy of 78.14% and 70.26%, respectively. Moreover, CNN model improves the both training loss and validation loss significantly.

# **Reference**
- Kaggle dataset: https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000

- Dataverse Harvard: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T

- Helpful links:
    + Teaching Machines to Detect Skin Cancer: https://medium.com/analytics-vidhya/teaching-machines-to-detect-skin-cancer-bd165566f0fe
    + Dermatology MNIST: Loading and Processing: https://kaggle.com/kmader/dermatology-mnist-loading-and-processing
