# Preprocessing Data
So now that you’ve gotten to see some brains, you may or may not be wondering: How do we compare different people’s brains when they are different sizes with their own quirks? Even if you weren’t wondering that, you will be receiving the answer: we preprocess it!

Preprocessing is when we warp, move, and reshape the brain to fit a template brain([MNI152](https://www.lead-dbs.org/about-the-mni-spaces/) is a commonly used one). What this does is “prepares” the data to be analyzed by having the same part of the brain in the same part of the image for all participants. 

In addition to correcting differences in shape, this process also corrects for any movement or other factors that introduce noise during functional scans. Another important step in this process is blurring. This is an optional step that depends on the analysis that will be ran on the data. 

At the end of this process, you will be able to point to one region of the brain at certain coordinates and be confident that it is the same region at the same coordinates in all other participants as well. You do not need to know extensively about how this is done(or battle through dense MRI textbook chapters on it like some people did…I’m some people in this case), but it is good to have a basic understanding of what goes into it. 

This video(first bullet) gives a detailed but, brief overview of what goes into this process and the web page(second bullet) is a good written description of it:

- [fMRI Analysis: Part 1 - Preprocessing](https://www.youtube.com/watch?v=xLWES956JJE)

- [Preprocessing of fMRI data](https://mafil.ceitec.cz/en/preprocessing-of-fmri-data/)

[fMRI and Artifact computation and Analysis](https://iopscience.iop.org/article/10.1088/1742-6596/1818/1/012083/pdf) by Nasser et al. does a great job of describing these concepts in a way that is easily understandable for someone new to the field. 

 ------------------------------------------------------------------------------------------------
 <div style="display: flex; justify-content: space-between;">
  <a href="viewing_data.md">Last Page - (Viewing Data)</a>
  <a href="data_management.md">Next Page - (Data Management Basics) </a>
</div>

<div style="text-align: center; margin-top: 10px;">
  <a href="home.md">Home</a>
</div>

