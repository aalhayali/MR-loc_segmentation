# MRI Localiser Prostate MRI Rectal Segmentation
This project segments the rectum from prostate MR-localiser images. 

***NOTE*** - This work is a portion of a project in collaboration with the University of Ottawa Hospital. Full research paper is currently under review.

# Clinical Background 
This study was approved by the local institutional review board with waiver of consent. 213 consecutive men (mean age of 64 +/- 7.7 years) referred for prostate MRI at a single academic referral center between January 2014 and March 2016 were included. Examination indications included: pre-biopsy, prior negative biopsy and active surveillance. Patients post-prostatectomy or pelvic radiotherapy and with hip prosthesis or other metallic implant were excluded. The data were available to the (BLINDED) through a data-sharing agreement. All patients underwent multi-parametric MRI at 3 Tesla using the same clinical system (Discovery 750W, GE Healthcare) at a tertiary care referral center for prostate. During the study dates, patients either underwent no preparation of a Fleet<sup>TM</sup> enema self-administered 3 hours prior to MRI.

Rectum was segmented by a medical imaging student working with a fellowship trained genitourinary radiologist with 10 years of post-fellowship experience in prostate MRI (BLINDED). The student and radiologist manually segmented the rectum from the anal verge to the sacral promontory (approximate level of the rectosigmoid junction) on all sagittal images in which the rectum was visible, using ITKSnap 3.8.0. Manual segmentation was performed on 213 patients.


# Dependencies
1. `Pytorch` - deep learning framework <sub>duh<sub>
2. [`nibabel`](https://pypi.org/project/nibabel/) - converting NIFTI volumes to NumPy arrays
3. [`albumentations`](https://pypi.org/project/albumentations/) - image augmentations
4. [`segmentation models`](https://github.com/qubvel/segmentation_models.pytorch) - Pytorch based segmentation models with pretrained backbones
5. `tqdm` - making loops look nice


**Personal note** - The nature of this project and collaborator's technical expertise prevented big chunks of the notebooks to be modularised. Enjoy!