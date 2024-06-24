# What is Neuroimaging Data?

This covers most of the essential knowledge needed for understanding what the data is and a preview of what it looks like.

[Principles of fMRI Part 1, Module 3: fMRI Data Structure & Terminology](https://www.youtube.com/watch?si=kYY_AHLALB6hqd4V&v=OuRdQJMU5ro&feature=youtu.be)

This web page helps explain further what exactly BIDS is (and make sure you buy some merch):

[Brain Imaging Data Structure](https://bids.neuroimaging.io)

Just to clarify, the data comes off of the scanner in the DICOM format (i.e., what your doctor uses), and then using a script of choice, it is converted to .nii files and organized in the BIDS structure. This will probably seem a little overwhelming at the moment, but [here is an example of one commonly used program to convert data from DICOM to BIDS/NIFTI format](https://github.com/rordenlab/dcm2niix).

An important note: these files are large. Very very large. While you can do some small projects using a good amount of .nii files on your local computer, most large projects store their data on a server that can be accessed remotely (or not in some cases). For anyone not familiar with computers, you are basically logging into another computer that is somewhere else from your computer. This can be done in a number of ways that I will save for another time.


 ------------------------------------------------------------------------------------------------
<div align="center"; margin-top="10px">
  <a href="unix_basics.md">Next Page - (Unix Basics) </a>
</div>

<div align="center"; margin-top="10px">
  <a href="README.md">Home</a>
</div>
