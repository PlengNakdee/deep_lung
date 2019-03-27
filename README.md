# Lung Nodule Classification Using Deep Learning

This deep learning project is a supervised learning, by training a model for lung nodule classification. There are two classes: cancer or not cancer. The process is as follow:

1. Download a LUNA16 from (https://luna16.grand-challenge.org/data/). The dataset is 888 images of CT scan.
2. The dataset filename is .mhd. So I convert them to .png (mhd_to_png.ipynb). After convertion, some images have too much noise or not in the same shape as others. I had to cut them out and I was left with 660 images.
3. Convert .png images to nparray (png_to_nparray.ipynb). Each images has a label: 1 means cancer, 0 means not cancer.
4. Save the arrays as x_images.npz and y_labels.npz and use them on Google Colab.
5. Using Google Colab, because it has a GPU, to creat a deep learning model. Training and testing. (lung.ipynb)
