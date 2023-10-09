# Mambaforge and devbio-napari

Before attending the course, please install mambaforge on your computer as explained in this [blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html). 

If you already have some conda or anaconda installation on your computer, ***please install mambaforge*** anyway as explained in the blog post linked above. 

Furthermore, please install [devbio-napari](https://github.com/haesleinhuepf/devbio-napari#installation) into a fresh conda environment, e.g. using this command:

```
mamba create --name devbio-napari-env python=3.9 devbio-napari pyqt -c conda-forge
```

When you are done, you can test your setup by executing these commands from the command line:
```
conda activate devbio-napari-env

naparia
```