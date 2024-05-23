# ActigraphyViViT

In this study, we evaluate the performance of various deep learning architectures, including the recently popularized Video Vision Transformer (ViViT), in analyzing actigraphy data, a key modality for understanding physical activity patterns, as collected through actigraphy monitors. Actigraphy is a powerful modality used in health-related research, and previous studies have shown robust results from understanding actigraphy data via convolutional methods. It is well established that reshaping actigraphy data into a video format yields the best results, with the current state-of-the-art model for actigraphy model being the ConvLSTM, which intakes video data. We aim to push the state of the art in actigraphy understanding by developing attention-based models for actigraphy understanding. We hypothesized that reshaping actigraphy data into a video would also be helpful for attention-based models, as this is the case for convolutional-based models. Our findings suggest the opposite. Our most robust 3D Video Transformer model, the pre-trained ViViT, performed significantly worse than our custom 1D Transformer models. Remarkably, however, the 1D Transformer models outperformed the ConvLSTM and set a new state-of-the-art benchmark for actigraphy understanding. We present a detailed comparison of these architectures, examining their performance on a large dataset sourced from NHANES, which includes roughly 300 million actigraphy data points sourced from 30,000 participants. The comprehensive study aims to identify the most effective model for actigraphy analysis, and also the most effective representation for actigraphy data: sequence or video. 

# Reproducible Notebooks Below


## Reproducible Notebook for Transformer (M): https://colab.research.google.com/drive/1Xp3s8Up6ko3kfXlPQrIFGQb5cMaUAiI0?usp=sharing
The model you will be running is the one under `Transformer_Medium_SmoothedData` <br> 
You have to connect to TPUv2, or this will NOT WORK <be>  
Go to runtime->change runtime type <br>
Then select TPUv2 <br>
You will need Colab Pro, but sometimes Google allows anyone to connect to their TPUv2 -- give it a shot!
