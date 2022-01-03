
1./Data Processor folder contains Python scripts to construct augmented training dataset in addition to Hateful Memes Challange dataset
Meme_Add Gaussian Noise.ipynb: Construct noisy meme images with Gaussian distribution and append to the original training dataset
Meme_Add Memotion 7K.ipynb: Select suitable Memotion 7K dataset, convert to MMF accepted format and append to the original training dataset
Meme_Replace Text with Similarities.ipynb: Construct "twisted" memes text with characters randomly replaced using Facebook Augly tool and append to the original training dataset

2. 
MMBT_Add Image Noise.ipynb: MMBT baseline training on training dataset augmented by Gaussian noisy memes images 
MMBT_Add Memotion 7K.ipynb:  MMBT baseline training on training dataset augmented by Memotion 7K dataset
MMBT_Add Text Replaced with Similar Characters.ipynb:  MMBT baseline training on training dataset augmented by "twisted" memes text with characters randomly replaced with similar languages/symbols
MMBT_Baseline.txt: MMBT baseline by default training on original training dataset per 5000 iterations
