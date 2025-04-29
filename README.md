# Deep Learning Final Project

Glaucoma is a group of progressive eye diseases characterized by the degeneration of retinal cells and their axons leading to irreversable vision loss. Glaucoma affects over 76 million people globally and has significant challenges to normal detection. A major challenge in glaucoma is that this disease can progress over time silently (or at least minimal symptoms) until vision loss has started to occur. Like most other diseases early detection is critical to slowing disease progression.

Detection of glaucoma involves multimodal assessments combining fundus imaging, tonometry, pachymetry, and visual field testing. However, manual assessment can be subjective and labor intensive which highlights the need for some automated reliable models. Structural changes suggesing disease progression can include cup to disc ratio (CDR) which is a measure of asymmetry between the eyes, neuroretinal rim thinning, peripapillary atrophy or disc hemorrhages etc.

Clinical data as well can be useful in diagnosis highlighting potential irregular values for risk factors. Some typical risk factors include elevated intraocular pressure (IOP), but can also include things such as optic disc cupping, pachymtetry (corneal thickness), axial length of the eye, and visual field mean deivation which comes from visual field testing. These clinical values can come from the imaging themselves or separate risk factors when combined with standard information such as age/gender etc.

Recent advances in machine learning and artificial intelligence have come up with models that look at imaging and have looked at clinical data. However, not much has been done on mixing the 2 approaches to overlay clinical data with the imaging to take a combination approach. Thus, the project here uses 2 different neural networks :

A convolutional neural network (CNN) that will analyze the fundus images and extract features
A feed forward neural network (FNN) that will process the clinical data
By merging these 2 modalities into a predictive model, we aim to improve diagnostic performance compared to image only or clinical information only approaches. The final model will be assessed on typical machine learning metrics of accuracy, AUC/ROC, and confusion matrix metrics.

The data acquired for this project was taken from the PAPILA dataset which was published in 2022 by Kovalyk et al in Nature Scientific Data (https://www.nature.com/articles/s41597-022-01388-1). The downloaded data was obtained from here : https://figshare.com/articles/dataset/PAPILA/14798004?file=35013982. The specific publication here was a simple ResNet50 image classification task, but our work here will attempt to combine the clinical variables to create a multimodal classification system.

