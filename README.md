<h1 align="center">Fine-tuning Facenet</h1>

Current project is built based on [this repo](https://github.com/timesler/facenet-pytorch).

## Step 1: Set up everything

1.1. Your file structure should be something like this:

```bash
/images
    /person_1
        img1.jpg
        img2.jpg
        ...
    /person_2
        img1.jpg
        img2.jpg
        ...
    ...
    /person_2
        img1.jpg
        img2.jpg
        ...
```

1.2. Import conda environment and activate it:
```bash
conda env create -f environment.yml
conda activate facenet_pytorch
```

## Step 2: 

Use mtcnn model to detect faces and save/store them, so that you can train them for face recognition. Run this file on your jupyter notebook:

```bash
detect_and_save_faces.ipynb
```

## Step 3: Start training (fine-tuning) facenet model
Just run:

```bash
train.ipynb
```

Set proper images directory and suitable batch size.
