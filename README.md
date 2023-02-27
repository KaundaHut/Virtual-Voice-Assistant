# Virtual-Voice-Assistant
This directory contains code to import and evaluate the speaker identification and verification models pretrained on the VoxCeleb(1 & 2) datasets as described in the following papers (1 and 2):
     [1] A. Nagrani*, J. S. Chung*, A. Zisserman, VoxCeleb: a large-scale speaker identification dataset, 
         INTERSPEECH, 2017

     [2] J. S. Chung*, A. Nagrani*, A. Zisserman, VoxCeleb2: Deep Speaker Recognition, 
INTERSPEECH, 2018
The models trained for verification map voice spectrograms to a compact Euclidean space where distances directly correspond to a measure of speaker similarity. Such embeddings can be used for tasks such as speaker verification, clustering and diarisation.
## Prerequisites
    [1] Matlab

    [2] Matconvnet.
## Installing
The easiest way to use the code in this repo is with the vl_contrib package manager. To install, follow these steps:

Install and compile matconvnet by following instructions here.

Run:
       vl_contrib install VGGVox
       vl_contrib setup VGGVox
You can then run the demo scripts provided to import and test the models. There are three short demo scripts. The first two scripts are for identification and verification models trained on VoxCeleb1. The third script imports and test a verification model trained on VoxCeleb2. These demos demonstrate how to evaluate the models directly on .wav audio files:
        demo_vggvox_identif 
        demo_vggvox_verif 
        demo_vggvox_verif_voxceleb2
 ## Models
 The matconvnet models can also be downloaded directly using the following links:

Model trained for identification on VoxCeleb1

Model trained for verification on VoxCeleb1

Model trained for verification on VoxCeleb2 (this is a resnet based model)

## Datasets
These models have been pretrained on the VoxCeleb (1&2) datasets. VoxCeleb contains over 1 million utterances for 7,000+ celebrities, extracted from videos uploaded to YouTube. The speakers span a wide range of different ethnicities, accents, professions and ages. The dataset can be downloaded directly from here.
## Citation
If you use this code then please cite:

    @InProceedings{Nagrani17,
          author       = "Nagrani, A. and Chung, J.~S. and Zisserman, A.",
          title        = "VoxCeleb: a large-scale speaker identification dataset",
          booktitle    = "INTERSPEECH",
          year         = "2017",
   }
    @InProceedings{Nagrani17,
          author       = "Chung, J.~S. and Nagrani, A. and Zisserman, A.",
          title        = "VoxCeleb2: Deep Speaker Recognition",
          booktitle    = "INTERSPEECH",
          year         = "2018",
}
