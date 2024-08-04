# What is an MRI and how does it work?

MRI stands for **Magnetic Resonance Imaging**, which probably doesn't mean much to you now but will by the end of this module! 

If you bet that I was going to actually be the one writing all of this material, then you would probably lose that bet. This article does a good job at explaining how an MRI works and if a lot of it doesn’t make sense, that is *okay*. You do *not* need to be an MRI physicist by the end of this but just have a basic idea of how we go from putting a person in the scanner to looking a pretty image of their brain:

**[Magnetic resonance imaging (MRI) (article) - Khan Academy](https://www.khanacademy.org/science/biology/human-biology/neuron-nervous-system/a/magnetic-resonance-imaging-mri)**

Now that you have read some about how an MRI works, these videos are great for reinforcing the concepts through helpful animations since not everyone intuitively imagines what proton precessions look like(by not everyone, I mean no one). The videos below are in order of increasing level of detail(aka the top is easiest and the bottom is the hardest) since there will be people with different levels of background knowledge.

- **[MRI in 10 Minutes!](https://youtu.be/jLnuPKhKXVM?si=K08V18WdL5oLSaco)** This is all you need. It can give you a basic idea of how exactly an MRI works. Since it would be pretty embarrassing to say you work with MRIs but when asked how they work, have no idea and pretend you do until you cave and admit to them you just work with the data and don’t know…who would ever get caught in that situation? 
- **[MRI in Just Under 10 Minutes!](https://youtu.be/1Ku6-uXw7Ag?si=eUFo5yEXmpEOQl4f)** This is a slightly less fun version of the video above, but it does do a better job at explaining the physics behind MRIs which for anyone who’s more of a math/science type of student.
- **[Super In Detail For the Engineers](https://youtube.com/playlist?list=PLkSVzqeK5v2C4X1G3IuRUQeNveNGNxZrn&si=2QvvOv37GIvj9gUC)**: Unless you have a strong physics and mathematics background and a few hours time, don’t bother torturing yourself with this(the lack of exclamation point in the title is telling). This is very in detail on the mechanisms/equations that drive how an MRI is taken. 

### Is it the MRI way or the highway? 

To make a long story short, *no*. MRI is a very useful imaging modality since it *does* ***not*** *expose the subject to radiation* like some other imaging modalities such as **PET**, **CT**, and **X-Ray**. Not only that, but it offers a good combination of *spatial resolution* and *temporal resolution*. 
  - **Spatial resolution** is a measure of how small of pieces we can break up the image into
      - It is the same as number of pixels used for a video or image
          - Having less pixels, such a 360p video, looks much blockier and blurrier than a high definition with more pixels, 1080p video
          - If you do not know what 360p and 1080p means, go on  youtube and look at the settings on the bottom right of your video. You can change the quality of the video to whichever you chose and will be able to see a visible difference in clarity
      - MRI's are 3D images that use **voxels** instead of pixels.
          - *Voxels* are just 3-dimensional pixels. They are the tiny cubes that each have a measured intensity from the scan, and therefore show up in the image with that intensity.
  - **Temporal Resolution** is a measure of how often you take your measurements.
      - For example, iff we want to track activity of the brain(which is a fast-changing process), it would be much better to have measurements every millisecond(higher temporal resolution) than every 20 seconds(lower temporal resolution). 
      

While MRI is a very versatile tool for imaging, some other important imaging methods such as **EEG**, **MEG**, and **PET** scans are also used and each has their own pros and cons(as previewed in the graphic *below*). As you continue to learn, you will see that some imaging methods are better suited for some types of studies. 

![Pro Con List of imaging methdos](docs/assets/images/imagingprocon.png)

Image from:

Mendez Orellana, Carolina. (2015). Functional MRI of Language Processing and Recovery. 
https://www.researchgate.net/publication/295856844_Functional_MRI_of_Language_Processing_and_Recovery. 


## Signal To Noise Ratio (SNR)
This is a concept important enough to get its own section, but I will preface it with this is one of the more difficult topics for some. 

So when we are measuring the intensity of the voxel, what we are able to read is not always the "true" or "exact" value since our measuring tools are not 100% accurate and there are other factors that can cause changes to the intensity we measure. We call the measurements that we take the *observed signal*. 

**SNR** is a representative of the magnitude of the observed signal(the stuff we are interested in, which in our case is the different intensity created by different bodily tissues) versus the magnitude of the noise(potentially caused by factors that could change the intensity of voxels like subject movement, magnetic field interruptions, etc.). I know most of you are not signal processing experts, but the image below does a good job at showing what this looks like for a 2D wave. 

In this example, we measured the line on the left. It has a similar structure to the true signal shown on the top right, but if we went to the same X coordinate on the observed signal and true signal, we would get slightly different values. This is due to the noise - the noise introduces slight variations. Think of the observed signal as the signal+noise.

![Image showing observed signal decomposed into signal and noise](docs/assets/images/noise.png)
*Image from https://www.predig.com/whitepaper/reducing-signal-noise-practice*

***So why do we care about SNR?*** Because we want to know that what we are seeing is actually from the signal we are measuring(brain activity) and *not* from random noise (which would mean the results are meaningless). 

***How do we even calculate SNR from an image?*** For most purposes, you will use a premade program to do this for you. There are equations to calculate this, but to spare your brain, I will leave it out of this introduction. 

I am not going to go more in depth on this topic, but it is important to have a good understanding of if you are going to be managing neuroimaging data. Many of the steps in the preprocessing of MRIs is done to improve SNR so we can be more confident in our results. 

<div style="text-align: left; margin-top: 10px;">
  <a href="fmri_bold_signal.html">Next Page (fMRI/The BOLD Signal)</a>
</div>

 <div style="text-align: center; margin-top: 10px;">
  <a href="/fmri-for-beginners/">Home</a>
</div>

