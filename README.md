# Deep Learning & Computer Vision Coursework

This repository collects a set of deep learning and computer vision notebooks I completed for college coursework. The assignments started as professor-given tasks, but I have kept them together here as a small personal project repo to show the range of models and workflows I practiced while learning modern CV.

The work is notebook-first and exploratory: each task includes data loading, preprocessing, model definition or fine-tuning, training loops, evaluation, and visual checks where relevant.

## Projects

| Notebook | Topic | What it covers |
| --- | --- | --- |
| `Task 1.ipynb` | Pet breed image classification | Custom PyTorch dataset setup, train/test splitting, training and evaluation loops, and comparison with pretrained CNNs such as ResNet50, AlexNet, GoogLeNet, and EfficientNet-B3. |
| `Auto-encoders + Task 2.ipynb` | Autoencoders and segmentation masks | Starts with MNIST reconstruction using linear and convolutional autoencoders, then applies encoder/decoder-style ideas to person mask generation with Dice and IoU evaluation. |
| `Task 3.ipynb` | Image captioning with LSTMs | Builds an image captioning pipeline using a CNN encoder, an LSTM decoder, vocabulary/token handling, teacher forcing during training, and caption generation for unseen images. |
| `Task 4.ipynb` | Vision Transformer for classification | Walks through ViT building blocks including patch embeddings, class tokens, positional embeddings, transformer encoder blocks, and training on the pet breed dataset. |

## Skills Demonstrated

- Building custom `Dataset` and `DataLoader` pipelines in PyTorch
- Training and evaluating CNN-based image classifiers
- Fine-tuning pretrained Torchvision models
- Implementing autoencoders for reconstruction and mask-style outputs
- Measuring segmentation quality with Dice score and IoU
- Combining CNN feature extractors with LSTM decoders for image captioning
- Implementing Vision Transformer components from scratch
- Visualizing model inputs, outputs, feature maps, losses, and predictions

## Tech Stack

- Python
- PyTorch and Torchvision
- NumPy and Pandas
- OpenCV
- Matplotlib and Seaborn
- scikit-learn
- torchmetrics
- spaCy
- Jupyter Notebook

## Datasets

The notebooks reference coursework datasets such as pet breed images, person segmentation data, MNIST, and Flickr8k-style image captioning data. The datasets are not included in this repository because of size and distribution constraints.

If you want to run the notebooks locally, place the required datasets in the paths expected inside each notebook, or update the path variables near the data-loading sections.

## How to Run

1. Clone the repository.
2. Create a Python environment with the dependencies listed above.
3. Install Jupyter:

   ```bash
   pip install notebook
   ```

4. Open the notebooks:

   ```bash
   jupyter notebook
   ```

5. Run each notebook after updating dataset paths as needed.

## Notes

This is not meant to be a polished production ML package. It is a learning-focused collection of assignments where I explored different parts of the deep learning and computer vision workflow, from classic CNN transfer learning to sequence generation and transformer-based vision models.
