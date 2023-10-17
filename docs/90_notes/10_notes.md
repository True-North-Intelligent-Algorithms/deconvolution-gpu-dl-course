## Collaborative Assignment

If you have any interesting answers, observations or thoughts about the below question please post on our Image.sc thread. 

1.  Were you able to run the deep learning training notebooks or did you run out of GPU memory?  Is it possible to get the training examples running by modifying the batch size or the size of the training patches?  How much memory is needed to train convnets for 3D applications as compared to 2D applications?  Do you have suggestions as to cloud computing services (such as AWS or other) that could be used to do deep learning training using high memory GPUs?  Post answers on workshop Image.sc thread. 

2. Re-run the ```restore_care``` network with all three pretrained networks 'cytopacq_noise_high_na_high' (a network trained on cytopacq nuclei), ```big_small_noisy_notnoisy``` (a network trained on big and small spheres but no nuclei) and 'combined' (a networks trained on several sphere images and nuclei).  How well can networks generalize?  What is the difference in results for the sphere (or nuclei) specific networks as compared to the combined?

3.  Look at the results of the ```restore_care``` and ```restore_stardist``` notebooks (if you couldn't run them look at the results on the online pre-run copies).  Do you notice a difference in quality of results between the images with large spheres in the center, and the images with medium sized spheres in the center?  You should notice that both restoration and segmentation of the peripheral spheres, were better when there was only a small sphere in the center.  Even though in both cases the size and brightness of the peripheral spheres were the same.  How do you explain this?

4.  Try to get better performance on the entire test set (especially the images with large spheres) by retraining the CARE and/or Stardist networks.  Some strategies that may help get better results.

* train for more epochs
* create new training images with more examples of large spheres and small spheres in the same image
* other?

5.  If you know of other deep learning and/or deconvolution toolkits that can be used to get better or more interesting results on these images, post these results on the workshop image.sc thread.   Especially of interest would be performance of 'segment anything' (SAM) models. 

6.  What is faster on the same image size?  Applying a CARE network, or 200 iterations of Richardson Lucy?
