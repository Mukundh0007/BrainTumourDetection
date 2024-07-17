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
<img width="913" alt="image" src="https://github.com/user-attachments/assets/1fe52fcf-22a4-4992-b1f4-2b9e9b35741a">

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
<img width="1024" alt="Screenshot 2024-07-17 at 11 44 55 PM" src="https://github.com/user-attachments/assets/e9677d99-332a-4c95-b6e9-cbf74dd1430c">

### Synergy with GEMMA 
By integrating the image classification model with GEMMA's text generation capabilities, we aim to bridge the information gap between technical diagnoses and patient understanding. The model not only classifies brain tumors but provides additional insights in a way patients can comprehend, promoting patient empowerment in their healthcare journey.
![image](https://github.com/user-attachments/assets/003caa3a-27be-4a95-bf99-2c9b8f6306d2)

![image](https://github.com/user-attachments/assets/b1289209-6c19-449d-aaea-61a9e28dea32)




##### References

• Naseer, A., Yasir, T., Azhar, A., Shakeel, T., & Zafar, K. (2021). Computer￾Aided Brain Tumor Diagnosis: Performance Evaluation of Deep Learner 
CNN Using Augmented Brain MRI. International journal of biomedical 
imaging, 2021, 5513500. https://doi.org/10.1155/2021/5513500 
• Sarhan, A. (2020) Brain Tumor Classification in Magnetic Resonance 
Images Using Deep Learning and Wavelet Transform. Journal of Biomedical 
Science and Engineering, 13, 102-112. doi: 10.4236/jbise.2020.136010. 
• Mahmud, M.I.; Mamun, M.; Abdelgawad, A. A Deep Analysis of Brain 
Tumor Detection from MR Images Using Deep Learning Networks. 
Algorithms 2023, 16, 176. https://doi.org/10.3390/a16040176 
• Saeedi, S., Rezayi, S., Keshavarz, H. et al. MRI-based brain tumor 
detection using convolutional deep learning methods and chosen machine 
learning techniques. BMC Med Inform Decis Mak 23, 16 (2023). https://
doi.org/10.1186/s12911-023- 02114-6 
• Xiong, S., Wu, G., Fan, X. et al. MRI-based brain tumor segmentation 
using FPGA- accelerated neural network. BMC Bioinformatics 22, 421 
(2021). https://doi.org/10.1186/s12859-021-04347-6
• Rajinikanth, V., Kadry, S., & Nam, Y. (2021). Convolutional-neural￾network assisted segmentation and SVM classification of brain tumor in 
clinical MRI slices. Information Technology and Control, 50 (2), 280-295. 
• Fouad, I. A. (2021). Developing a fully automated CAD tool for effective 
and accurate detection of brain tumors in MRI images. International 
Journal of Computer Science and Information Security, 19(1), 1-9. 
• Anagun, Y. Smart brain tumor diagnosis system utilizing deep 
convolutional neural networks. Multimed Tools Appl 82, 44527-44553 
(2023). https://doi.org/10.1007/s11042-023-15422-w
Project Report 12
• ZainEldin H, Gamel SA, El-Kenawy EM, Alharbi AH, Khafaga DS, Ibrahim 
A, Talaat FM. Brain Tumor Detection and Classification Using Deep Learning 
and Sine-Cosine Fitness Grey Wolf Optimization. Bioengineering (Basel). 
2022 Dec 22;10(1):18. doi: 10.3390/bioengineering10010018. 
• Chen, T., Hu, L., Lu, Q., Xiao, F., Xu, H., Li, H., & Lu, L. (2023). A 
computer-aided diagnosis system for brain tumors based on artificial 
intelligence algorithms. Frontiers in Neuroscience, 17, 1120781. doi: 
10.3389/fnins.2023.1120781
