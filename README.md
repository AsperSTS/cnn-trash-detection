# Waste Classification with CNNs

Computer vision project for classifying waste images into six categories using a convolutional neural network.

The repository includes preprocessing, training, visual comparison of image transformations and a small inference interface.

## Categories

- Organic / biological waste
- General waste
- Metal
- Paper and cardboard
- Plastic and textile
- Glass

## Workflow

```text
raw images
   ↓
preprocessing and balancing
   ↓
CNN training
   ↓
metrics and experiment outputs
   ↓
model inference
```

## Main components

- `image_pipeline.py` — preprocessing, balancing and resizing.
- `train.py` — CNN training and experiment logging.
- `image_comparison.py` — Streamlit interface for comparing original and processed images.
- `useModel.py` — local model inference interface.

## Results

Experiment outputs and graphs are stored in the `graficas_*` directories for different training stages and GPUs.

## Installation

```bash
pip install -r requirements.txt
```

Dataset paths must be configured for the local environment before training.

## Run

Train the model:

```bash
python train.py
```

Compare preprocessing results:

```bash
streamlit run image_comparison.py
```

Run the inference interface:

```bash
python useModel.py
```

## Stack

Python · TensorFlow/Keras · OpenCV · NumPy · Streamlit · Matplotlib

## Scope

This is an experimental computer-vision project. Reproducing the exact training results requires the same dataset split, preprocessing configuration and environment used for each experiment.
