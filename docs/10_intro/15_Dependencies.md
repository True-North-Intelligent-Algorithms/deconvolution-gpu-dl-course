# Dependencies

Before installing the rest of the dependencies make sure you are in the new devbio-napari based environment you created in the last section.  Type the following.

```
mamba activate decon-dl-env
```

## Cuda and Cupy

Note: You can probably use a version different than 11, just make sure cudatookkit and cupy versions are compatible.

```
mamba install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
pip install cupy-cuda11x
```

## tnia-python and clij2-fft

The tnia-python library is used for projections and some helper functions, clij2-fft is used for deconvolution, and psfmodels is used for diffractions based PSFs. 

```
pip install tnia-python
pip install clij2-fft
pip install psfmodels
```

## Stardist and CSB Deep 

These libraries are used for deep learning and require Tensorflow.  For Windows we need to install tensorflow<2.11.  The tensorflow version (<2.11) is not required for Mac or Linux. 

```
pip install "tensorflow<2.11"
```

Then install stardist which should also install CSBDeep

```
pip install stardist
```

## raster-geometry

Raster-Geometry is used to generate simulate images for deconvolution testing and deep learning training.

```
pip install raster-geometry
```

## Additional for Mac and Linux users

Mac-users may also need to install this:

```
conda install -c conda-forge ocl_icd_wrapper_apple
```

Linux users may also need to install this:

```
conda install -c conda-forge ocl-icd-system
```


