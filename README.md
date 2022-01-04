# Doc

This repo contains all the code and report for the Deep Learning course project: Hateful_Memes_Detection.

## Project Introduction

Hateful contents that hurt a benign cyber public space sometimes comes in as multimodal memes that involve both image and text. Recent advances in multimodal machine learning provide capable models to detect hateful contents across multiple modalities. Building upon Facebook's baseline models in the Hateful Memes Challenge, this project explored meaningful methods in deep learning including data augmentation, semi-supervised self-training and model architecture to improve the performance of baseline models.

## Code
1./Data Processor folder contains Python scripts to construct augmented training dataset in addition to Hateful Memes Challange dataset
Meme_Add Gaussian Noise.ipynb: Construct noisy meme images with Gaussian distribution and append to the original training dataset
Meme_Add Memotion 7K.ipynb: Select suitable Memotion 7K dataset, convert to MMF accepted format and append to the original training dataset
Meme_Replace Text with Similarities.ipynb: Construct "twisted" memes text with characters randomly replaced using Facebook Augly tool and append to the original training dataset

2. MMBT_Add Image Noise.ipynb: MMBT baseline training on training dataset augmented by Gaussian noisy memes images

3. MMBT_Add Memotion 7K.ipynb:  MMBT baseline training on training dataset augmented by Memotion 7K dataset

4. MMBT_Add Text Replaced with Similar Characters.ipynb:  MMBT baseline training on training dataset augmented by "twisted" memes text with characters randomly replaced with similar languages/symbols

5. MMBT_Baseline.txt: MMBT baseline by default training on original training dataset per 5000 iterations

7. Self_Training_Pseudo_Label_Generation.ipynb: Pipeline for training on the RedditMemes dataset using a pretrained MMBT model on HatefulMemes dataset, the pesudo labels of which are later used for a retraining.

## Report
Hate_Memes_Detection_Report is the final report that includes five parts: introduction, methodology, experiment results, future works and referrence.
