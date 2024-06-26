# Introduction To fMRI Analysis Programs

So depending on how much of the theory part you’ve gone through, you’ll know that there are several different ways to analyze fMRI data. It largely depends on your research question, study design, and to an extent, personal preference. While it would be a great time to go through all of the different analyses and programs, what I am going to do instead is list a few programs that I am familiar with along with a brief introduction to them. Many of these programs do the same thing in slightly different ways, so certain aspects of each program may be considered “better” for certain processing or analysis steps. There is also the personal preference of the research group/institution that plays a big role in which program is used.

- [SPM](https://www.fil.ion.ucl.ac.uk/spm/software/spm12/): A GUI based program to conduct analyses. Good for someone who is just starting out due to the simplicity of the GUI, but requires MATLAB. Also has conn toolbox as an adjunct
- [AFNI](https://afni.nimh.nih.gov/): The swiss army knife of analysis programs. Mostly done through shell scripts although there is a GUI
- [Freesurfer](https://surfer.nmr.mgh.harvard.edu/): Good for surface based analyses/cortical thickness among many other things.

So you may be thinking: *What now? You just listed these programs rather vaguely?* And to satisfy your curiosity, here is the holy grail of neuroimaging, [Andy’s Brain Book](https://andysbrainbook.readthedocs.io/en/latest/). This website has several incredibly helpful, easy-to-follow **tutorials** on using various neuroimaging analysis programs.  Below, I will link the tutorials for the aforementioned programs(*which are just the ones that I am personally most familiar with, there are many others out there that are also very useful*) so that you can familiarize yourself with how to use them.


- [SPM: Start to Finish](https://andysbrainbook.readthedocs.io/en/latest/SPM/SPM_Overview.html)
- [AFNI: Start to Finish](https://andysbrainbook.readthedocs.io/en/latest/AFNI/AFNI_Overview.html)
- [FreeSurfer Short Course](https://andysbrainbook.readthedocs.io/en/latest/FreeSurfer/FreeSurfer_Introduction.html)

## Troubleshooting

It is an <u>*unavoidable fact*</u> that you will run into errors/problems when trying to use these programs. Some of them will be small mistakes on your end, some will be due to different operating systems, and some will remain a mystery until the end of time. Regardless of the problem’s origin, it is important to know how to solve these problems on your own. Andy’s Brain Book is always a good place to start, but when that fails:

- <u>**Google**</u>: Just because this is research, doesn’t mean you have to answer your questions differently than normal. Either paste in the error message or type your best description of the problem/error and hope you find something useful
- <u> **Documentation**</u>: Every(at least most) program has extensive guides outlining how to use different functions or scripts within it. Many times, you can just google "documentation for {the program you are using}" or "help {function you are using - this is mostly for afni}" and find some guidance.
- <u> **Message Boards**</u>: Many of these programs acknowledge that there are many problems out there and made message boards exactly for that reason. You can look to see if someone has had that same issue(by searching in the same manner as described above for Google) and see the answer given, or you can post a question of your own and hope it gets answered in a timely manner.
- <u> **Reach out to lab/team members**</u>: Don’t be afraid to ask for help! Like you, everyone had a learning phase where they needed some guidance. Many times, you will find that someone you work with will have a solution or suggestions to try.
-  <u> **Walk Away in Shame**</u>: This is only half serious, maybe even only a quarter. But like everything else in life, sometimes you need to take a step away and return to it with a fresh set of eyes(maybe not everything in life). Many times, it will be one small error that you should have caught earlier but were too caught up in your line of thinking to notice. Really, taking a break and coming back makes a difference(and neuroscience has proved it)!
-  <u>***ChatGPT***</u>: This one may be a controversial one, which is why I put it at the end, but in my opinion this is the most useful tool for any student(in any field) when used correctly. I want to emphasize the ***correctly*** on this; you can use ChatGPT to teach you in a very efficient way, but you also need to know how to prompt it so that you can use it to learn and quickly solve your problem rather than sift through a long text output. <u>Most Importantly</u>, always check with your PI/grad student/other supervisor about what they are and are not okay with you using ChatGPT for - this is for data security. Here, I am going to outline how I would go about solving some common problems using ChatGPT:
    - **FACT CHECKING**: When using ChatGPT(and most social media), the biggest mistake people make is to automatically believe what is given to them without a clue of its validity. ChatGPT is very impressive and provides lots of accurate, useful knowledge, but it is not perfect. It is especially not perfect when it comes to dealing with new problems or ideas, which is the crux of innovative research. So when prompting ChatGPT about trying new things, remember to always take it with an extra grain of salt. However, when just using ChatGPT to learn about things that have already been documented, you can request sources from ChatGPT which is a good first pass for ensuring what you are seeing is accurate. Despite this, should always follow it up by checking for the facts in academic journals or other reputable sources(with a simple search on a database/[Google Scholar](https://scholar.google.com/)/etc). This is most important when using ChatGPT to learn about topics rather than when using it for troubleshooting errors.
    - **Program Throws an Error**: Most of these programs will give an error in the command line of whatever environment is used to run it(in layman’s terms, whatever you use to run the program, like matlab or the command line, is where you will see the error). Copy and paste the error into ChatGPT and mention the program you are using along with any other details from the analyses that could be relevant to what the error says. If the answer is irrelevant, then do your best to summarize what the error is trying to say.
    - **Code Error**: Very similar idea to what’s above, but now you can copy the lines of code or your whole script, and then paste it in chat, followed by “this code gave me the following error, can you help me solve it:” and then copy and paste the error. You can also specify if you want it to point out the error and just say what to fix or to rewrite the code itself(which is great for someone new to coding/new to the func.tons being used, but keep in mind that sometimes the solution is inefficient/convoluted.
    - **Unknown Terms/Regions**: You can just say “can you please tell me about x as if I’m an y” where you replace x with the term/concept and y with a level of experience that you think best represents you
        - Example: As an engineering student, I know my math, so I may ask ChatGPT to explain to me how fourier transform works by prefacing it with “can you explain to me the math behind it, along through an electrical engineering lens”. If I want a more fundamental answer I may say “can you explain to me the math behind fourier transform as if I am a middle school student.”


 <div style="display: flex; justify-content: space-between;">
  <a href="statistics.html">Last Page - (Statistics)</a>
  <a href="coding.html">Next Page - (Useful Coding Skills) </a>
</div>

<div style="text-align: center; margin-top: 10px;">
  <a href="/fmri-for-beginners/">Home</a>
</div>
