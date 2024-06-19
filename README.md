# fMRI-Based Cognitive Neuroscience for Beginners

A complete course to learn both practical skills and theory involved in fMRI research.

By Sam Rosenberg  
Heavily borrowing material from Cory McCabe, and relying heavily on lectures provided through MIT Free Open Courseware, tutorials from Andy’s Brain Book, and various other sources

I am creating this “course” for someone new to/interested in this field to be able to both:
- Gain practical skills to use for research 
- Learn theory behind some of the analyses

I have not been involved much in data acquisition, so sadly none of that will be included. Instead, this is more focused on the data management, processing, and analysis side to provide information on everything to do once the data is on a server. 

If you have made it this far, I am going to assume you have the knowledge of a college student who’s taken most of their introductory science classes, but realistically, you can teach yourself all the knowledge needed to get involved. The internet in 2024 is a goldmine of free knowledge, just a goldmine that has several obstacles in the way of the gold and lot’s of fools gold mixed in. That’s why this guide sticks to reputable sources and makes your life less stressful.

I will split this into both theory and practical knowledge. You do not need to go through all the theory to understand a good deal of the practical knowledge, but in the practical knowledge I will use terminology introduced in the theory material that will expect the reader to know what it is (or can look up what it is which is what I personally would do). 

## Contents

- [Theory](#theory)
  1. [How an MRI works](#how-an-mri-works)
  2. [fMRI/The BOLD Signal](#fmri-the-bold-signal)
  3. [HRF (Hemodynamic Response Function)](#hrf-hemodynamic-response-function)
  4. [GLM (General Linear Model)](#glm-general-linear-model)
  5. [Neuroanatomy](#neuroanatomy)
  6. [More General Methods Background](#more-general-methods-background)
  7. [More to come](#more-to-come)

- [Practical Knowledge/Skills](#practical-knowledgeskills)
  1. [What is neuroimaging data?](#what-is-neuroimaging-data)
  2. [Unix Basics](#unix-basics)
     - [File Permissions](#file-permissions)
     - [Transferring Files Between Servers](#transferring-files-between-servers)
  3. [Viewing Data/Drawing VOIs/Lesions](#viewing-datadrawing-voislesions)
  4. [Preprocessing Data](#preprocessing-data)
  5. [Data Management Basics](#data-management-basics)
  6. [Statistics](#statistics)
  7. [Introduction To fMRI Analysis Programs](#introduction-to-fmri-analysis-programs)
     - [Troubleshooting](#troubleshooting)
  8. [Useful Coding Skills](#useful-coding-skills)
  9. [Practice](#practice)

- [List of Resources](#list-of-resources)