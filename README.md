# Road-Feature-extraction-from-Satellite-Imagery

For road feature extraction from satellite image following thing were explored
  - Data analysis. There were 301 missing label from the 1024 training images.So the training data was split into train/val and unlabelled data. 
  - Literature survey was done to evaluate the different models.DLinknet which was found to be a good model for road surface extraction. 
  - DLinknet and Efficinet Unetb4 is condisered for this experiment. 
  - While training D4 augmentation and than more augmentation technique were used. 
  - Dice loss and binary cross entropy loss are used for training. 
  - Iou score, Precision, recall and F1 score are used for model evaluation. 
  - Adam optimizer and CosineAnnealingWarmRestarts scheduler 
  - Pseudo labelling for unlabelled data was for training


### Requirement
-pytorch
-requirement.txt
-[segmentation model pytorch api](https://github.com/qubvel/segmentation_models.pytorch).
-[albumentations](https://github.com/albumentations-team/albumentations).
-[Dlinknet](https://github.com/zlkanata/DeepGlobe-Road-Extraction-Challenge).
-[utilit library](https://github.com/BloodAxe/pytorch-toolbelt).
-[Training pipeline](https://github.com/catalyst-team/catalyst).


### Results
![Alt text](Output.PNG?raw=true "Inference")

### Pseudo Labelling
![Alt text](PseudoLabelled.PNG?raw=true "Inference")

### TO Do
- TTA 
- SWA
- Tile based processing
- Focal loss/Lovasz loss
