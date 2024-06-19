# Comparative analysis of Machine Learning algorithms for predicting the stereotactic coordinates of the Centromedian nucleus from a T1w MRI image
Introduction: Deep brain stimulation (DBS) of the centromedian nucleus (CM) of the thalamus is a promising treatment for drug-resistant epilepsy (DRE), Gilles de la Tourette syndrome, pain, and disorders of consciousness, particularly when other surgical options are not feasible. However, the CM is challenging to visualize on routine MRI and atlas based targeting often results in inaccurate electrode placement, affecting surgical outcomes. Inability to visualize and directly target the CM remains the biggest barrier to entry for CM-DBS in a resource limited setting. 

Methods: We developed and tested machine learning (ML) models to predict the stereotactic coordinates of the CM using input features, which were x,y and z coordinates of readily identifiable points from T1-weighted (T1w) MRI images. Four ML models—Linear Regression (LR), K-Nearest Neighbor (KNN), Support Vector Regression (SVR), and Deep Neural Networks (DNN)—were trained and optimized using 100 MRI scans from the Human Connectome Project (HCP). Models were trained to predict coordinates of the centroid of the CM. Errors were defined as 3-dimensional distances between: known coordinates of CM from Krauth/Morel atlas and predicted coordinates from the ML models. Euclidean error was taken as the shortest distance between these two points in space. Models were validated using a dataset of 20 patients with generalized epilepsy, a frequent indication for CM DBS.

Results: The DNN model demonstrated the highest accuracy in predicting CM coordinates, with mean Euclidean error of 0.88 ± 0.41 mm in the HCP dataset, and 1.12 ± 0.44 mm in the epilepsy dataset. The LR, SVR, and KNN models also performed similarly, however with slightly higher error rates. 

Conclusion: Our study indicates that ML models, particularly DNNs, can accurately predict CM coordinates using standard T1w MRI images. This approach reduces the dependency on advanced imaging techniques, making CM-DBS more accessible.
