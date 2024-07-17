# BrainTumourDetection
Many patients lack direct access to and understanding of their medical imaging data. This can lead to feelings of uncertainty and hinder their ability 
to participate actively in their care. There is a need for a platform that empowers patients to engage with their medical scans while also streamlining the 
diagnostic process for healthcare providers.

A brain tumor is a collection, or mass, of abnormal cells in your brain. Your skull, which encloses your brain, is very rigid. Any growth inside such a 
restricted space can cause problems. Brain tumors can be cancerous (malignant) or noncancerous (benign). When benign or malignant tumors 
grow, they can cause the pressure inside your skull to increase. This can cause brain damage, and it can be life-threatening. 
This dataset is a combination of the following two datasets : 
• figshare
• SARTAJ dataset

This dataset contains 7023 images of human brain MRI images which are classified into 4 classes: glioma - meningioma - no tumor and pituitary.No 
tumor class images were taken from the Br35H dataset. 

The train and test split ratio is around 80:20, with 5712 images in train and 1311 images in test.

### Strengths of Convolutional Neural Networks (CNNs): 
• Feature Extraction: CNNs excel at automatically learning relevant 
features directly from image data. This is crucial for brain tumor 
classification, as identifying subtle patterns and textures within the 
MRI scans is paramount for accurate diagnosis. 
• Spatial Invariance: Through pooling layers, CNNs can achieve 
spatial invariance. This means the model can recognize tumors even if 
their location within the MRI slightly varies. This robustness is essential 
for real-world applications where image acquisition might not always 
be perfectly standardized. 


### Rationale for Including a Long Short-Term Memory (LSTM) Layer: 
We introduced an LSTM layer to investigate its potential benefits in these 
specific ways: 
• Capturing Sequential Relationships: MRI scans often consist of 
multiple slices that capture different sections of the brain. The LSTM 
layer, with its ability to process data in a sequential manner, can learn 
subtle relationships between these slices that might be informative for 
tumor classification. 

### Synergy with GEMMA 
By integrating the image classification model with GEMMA's text generation capabilities, we aim to bridge the information gap between technical diagnoses and patient understanding. The model not only classifies brain tumors but provides additional insights in a way patients can comprehend, promoting patient empowerment in their healthcare journey.
