# computer-vision-dscuwa
Crash course in modern computer vision for Data Science Club of UWA.

## Setup

Using [minicoda](https://www.anaconda.com/download/success) (or your preferred virtual environment), create a new environment:
```
conda create -n cv-demo python=3.10
conda activate cv-demo
```

Install this project's dependencies:
```
pip install -r requirements.txt -e .
```

## 1. Basics and classical CV

Start simple. If you can solve your problem with these approaches, you can avoid maintaining and versioning datasets and models.
These approaches start to fail when tested on a wider variety of data.

## 2. Convolutional Neural Networks

CNNs work well for identifying local details and determining relationships between a variety of features.
Can typically produce acceptable results with limited data (100s of images if using pre-trained encoders).
These approaches struggle with global details, hence most architectures include multiscale tricks (e.g. U-Nets, PSPNets).

## 3. Vision Transformers

ViTs naturally capture global dependencies between local image patches, but typically are larger models hence they tend
to be slower and require more data than CNNs. They have the advantage of naturally translating between different
modalities (image, text, audio). If you're working on a project with large, labelled datasets, then ViTs may be a good solution.

## 4. Self-paced Project

The best way to learn is by doing. Create a challenge for yourself, find/create a dataset, and try to solve your problem!
Also makes for a great discussion point during interviews if you haven't had significant work-experience.
