# Steganography for Text: Hiding text messages inside images

## What is steganography?

> [Steganography](https://en.wikipedia.org/wiki/Steganography) is the practice of concealing a file, message, image, or video within another file, message, image, or video.

Inspired by this [excellent blog post](https://towardsdatascience.com/steganography-hiding-an-image-inside-another-77ca66b2acb1) explaining a simple approach for concealing one image within another image, I have created this small application to hide a text message inside a given image.

**This application requires an image with 3 channels (e.g. RGB) hence grayscale images will not work**

#### For a detailed explanation using a [Jupyter Notebook](https://github.com/DebalB/my-blogs/blob/master/_notebooks/2020-06-28-steganography_text.ipynb) refer to my [blog post](https://debalb.github.io/my-blogs/fastpages/jupyter/2020/06/28/steganography_text.html).

## Usage

Install the requirements:

```
pip install -r requirements.txt
```

Hide and Unhide your images with:

```
python steganography.py merge --img1=res/img1.jpg --img2=res/img2.jpg --output=res/output.png
python steganography.py unmerge --img=res/output.png --output=res/output2.png
```
