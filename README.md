# image-classifier

## CIFAR-10 Image Classifier

This project builds and evaluates a convolutional neural network in PyTorch using the `CIFAR-10` dataset. The goal is to compare an in-house image classification model against Detectocorp’s claimed `70%` benchmark accuracy and make a build-vs-buy recommendation.

## Project Summary

The notebook completes the following tasks:
- Loads and augments the CIFAR-10 training data
- Explores image dimensions, classes, and sample images
- Builds a CNN classifier with convolution, batch normalization, pooling, and dropout
- Trains the model and plots the average training loss per epoch
- Evaluates performance on the test set
- Saves the trained model weights for reuse

## Verified Result

After training for `6` epochs, the model achieved:

- **Test accuracy:** `71.53%`
- **Saved weights:** `cifar_classifier.pth`

This result slightly exceeds Detectocorp’s `70%` benchmark.

## Recommendation

Based on the measured test accuracy, the recommendation is to **build the solution in-house** rather than buy the external model. The classifier already performs slightly better than the proposed third-party benchmark, and it provides a solid baseline that can be further improved through hyperparameter tuning, longer training, or transfer learning.

## Files

- `CIFAR-10_Image_Classifier-STARTER.ipynb` — completed notebook
- `cifar_classifier.pth` — saved trained model weights
- `requirements.txt` — Python dependencies

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Open `CIFAR-10_Image_Classifier-STARTER.ipynb` and run the cells in order.
