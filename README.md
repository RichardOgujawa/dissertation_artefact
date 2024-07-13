# Dissertation Artefact

This is a repository for the coding artefact related to Richard Ogujawa's dissertation relating to comparing and contrasting GANs vs simple data augmentation techniques to investigate the impact of either approach.

A CNN model was trained on to accurately classify handwritten digits. The model was trained on MNIST data.

## _Evaluation_:

Three types of training datasets were used to train different models using the same model architecture and the performance for each model was evaluated by measuring the test and training accuracy.

### _First type_:

The orignal performance was evaluated by measuring the training accuracy (categorical loss) and testing accuracy (validation categorical loss).

![Original Data Model's Results](https://github.com/RichardOgujawa/dissertation_artefact/blob/main/images/history10_og.png)

![Original Data Model's Results](https://github.com/RichardOgujawa/dissertation_artefact/blob/main/images/history8_og.png)

- _Second type_: Then the training data was augmented using the images transformations cropped to only show the subject of interest (the digits).

![Data Augmented Model's Results](https://github.com/RichardOgujawa/dissertation_artefact/blob/main/images/history10_aug.png?raw=true)

![Data Augmented Model's Results](https://github.com/RichardOgujawa/dissertation_artefact/blob/main/images/history8_aug.png?raw=true)

- _Third type_: The _training data was augmented using DCGAN_ generated handwritten images. The DCAN generated images were the best ten generated images from each label class (0, 1, 2, 3..., etc.) These can be found in the directory labelled 'dcgan_generated_images'.

<!-- ![Data Augmented Model's Results](https://raw.githubusercontent.com/RichardOgujawa/dissertation_artefact/main/images/history10_aug.png)

![Data Augmented Model's Results](https://raw.githubusercontent.com/RichardOgujawa/dissertation_artefact/main/images/history10_aug.png) -->

- _Fourth type_: Similar to type four, but this time using _WGAN-GP_.
