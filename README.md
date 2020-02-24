![logo](scikit-image-logo.png)

# scikit-image notes

## contents:
- README.md

### user guide (jupyter notebook files)
- __crash course__ (NumPy indexing, color images, coordinate conventions, array dimension ordering)
- __image datatypes__ (inputs, outputs, working with openCV, pipelines, intensity rescaling, negative value clipping)
- __image adjustments__ (painting with labels, segment joins, RAG thresholding, contrast, exposure, histogram equalization)
- __working with video_files__ (ffmpeg hacks MoviePy, imageio)
- __simple tutorials__ (image segmentation, parallelization with joblib)
    
### gallery of examples (jupyter notebook files)
- __std image library__ (specific, scientific, general-purpose images)
- __NumPy operations__ (image manipulations, block views)
- __exposures & color channels__ (10 examples)
- __edges & lines__ (13 examples)
- __geometrical transforms & registration__ (13 examples)
- __filtering & restoration__ (13 examples)
- __feature & object detection__ (17 examples)
- __object segmentation__ (24 examples)
- __longer-form examples__ (8 examples)
- __developer exercises__ (advanced, 2 examples)

### issues / to-dos:
1) in gallery/longform.ipynb:
    - "face classification with haar-like feature descriptor" originally used the Dask library for task parallelization. I need to revamp the code to run on Jupyter notebooks. Error msgs are left in place for illustration.
    
2) in gallery/object-segmentation.ipynb:
    - "region adjacency graphs (RAGs)" is return an attribute error as follows: 'RAG' object has no attribute 'node'. this is caused by a break in networkx package version 2.4; change attribute 'node' to 'nodes' to fix it. (done.)