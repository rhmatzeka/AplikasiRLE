# Image Compression with Run-Length Encoding (RLE)

An interactive Jupyter notebook that compresses an image using **Run-Length Encoding** and shows you exactly what happened: the image before and after, the file size saved, and how the colors changed.

This was the final project for a Digital Image Processing course.

## What is RLE?

Run-Length Encoding replaces repeated values with a count. For example, `AAAABBB` becomes `4A 3B`. Images with large areas of the same color shrink a lot, while very detailed photos shrink less.

## What the notebook does

1. You **upload an image** with a button.
2. It **encodes** the pixels with RLE and **decodes** them back to check nothing was lost.
3. It shows the **original and reconstructed image** side by side.
4. It draws **RGB histograms** before and after.
5. It reports the **size before and after** and the **compression ratio**.
6. You can **download the RLE result** as a `.txt` file.

## Getting started

You need Python 3 and Jupyter.

```sh
pip install numpy pillow matplotlib ipywidgets notebook
jupyter notebook "Pertemuan 11/tugasakhir.ipynb"
```

Run the cell, pick an image, then click **Proses RLE** to process it.

## Tech stack

Python, NumPy, Pillow, Matplotlib, ipywidgets
