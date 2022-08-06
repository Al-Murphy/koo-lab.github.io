
_____________________________________________________________
## Meetings


https://docs.google.com/spreadsheets/d/11zZ7LSRaufHQN3ap9UEU17rL0EJ5hv0FJgVBeJTaLgM/edit#gid=337277395


* Koo lab zoom: https://zoom.us/j/98098694405?pwd=c0l1ME1WYlcwUGh5b042U0lVcTh2Zz09
* Super group zoom: https://us06web.zoom.us/j/87585929668?pwd=ZWc2M1B6bGtkcHM5MWp2REdwaDZ4Zz09

* One-on-one zoom:   https://zoom.us/j/92359312723?pwd=eVlkQjcwcnA1R2NuUmUybC9LaVIrQT09



- Group course (every other Fri at 3p) -  Amber
	- DL/RL summer school


_____________________________________________________________
## Socials

*QB happy hour* occurs every other Friday at 5p at Hillside patio (unless specified otherwise). It is a great opportunity to interact with the broader QB community. 

*QB Tea* takes place every Wednesday at 3-4p. Complimentary refreshments (i.e. Coffeee and Teas) as well as an assortment of treats (i.e. homemade cookies, brownies and fruit) are served. It is also a great opportunity to interact with the broader QB community.  


_____________________________________________________________
## Lab communications


#### Slack

- The *Koo lab slack channel* is the primary mode of communication in the lab. Relevant channels include #general, #random (for jokes), s#ocial (for planning social events), stay up to date with papers (via #papers-genomics, #papers-protein, #papers-dl), or as the lab #questions (about research questions). We also have a dedicated channel for questions about the #server. During virtual conferences, we can live chat on #conference_chat.

- *QB slack channel* is a fairly inactive workspace but occasionally important posts come through. It connects us to the broader QB community and so is worth being on. 

- *Elzar slack channel* is a place to ask questions about the CSHL servers. We use this to get guidance on using Elzar (i.e. submitting jobs, monitoring jobs, and troubleshooting).

_____________________________________________________________
## Servers

In addition to Elzar, the Koo lab has 4 GPU servers:

comet -- 143.48.35.36 -- 10 2080ti RTX GPUs
citra -- 143.48.44.146 -- 8 A4000 GPUs
simcoe -- 143.48.108.53 -- 2 Titan RTX GPUs
strata -- 143.48.108.92 -- 2 2080ti RTX GPUs

In order to access the servers, please contact Jakub (or me). 

To submit a job to a specific GPU, use this command:
	$ CUDA_VISIBLE_DEVICES=1 jupyter notebook --no-browser --port=8888
	
	ssh -N -L 8888:localhost:8888 peter@strata


Elzar

_____________________________________________________________
## Lab notebook

Staying on top of your research means being organized. Keeping a well-maintained lab notebook is crucial to transfer the mental map of dynamic research projects onto a platform that can help to remember key results and plan for the future. People in the lab use Evernote (including me) or ?. Try them out! I will not monitor your lap notebook habits but from personal experience, it is clearly the difference between who is on top of their research versus those that are scatterbrain -- keep forgetting next steps and forget where important documents/notes are. y


_____________________________________________________________
## Seminars


#### CSHL-based seminar series
 QB Seminar (Wed at noon), CSHL Labwide Seminar (Thu at noon), and the CSHL In-house Seminar (Fri at noon



#### External seminar series (virtual)

* _Machines, Inference and Algorithms series -- Broad Institute_
([Video](https://www.youtube.com/playlist?list=PLlMMtlgw6qNjROoMNTBQjAcdx53kV50cS)) 
* _DL Paper Reviews by Yannic Kilcher_
([Video](https://www.youtube.com/c/YannicKilcher/videos)) 
* _RNA-COSI Journal Club_ ([Link](https://irnacosi.org/journal-club/))




_____________________________________________________________
## Conferences 


- CSHL: Systems Biology: Global regulation of gene expression (Mar 9-12)
- ICLR (Apr 25-29) 
- CSHL: Biology of Genomes (May 10-14) -- Deadline Feb 18
- ISMB (Jul 10-14) -- Deadline Apr 21 
	- Shush/Amber (virtual)
	- Ethan/Rohit (virtual)
- ICML (Jul 17-23)  
- CSHL: Epigenetics and Chromatin (Sep 20-24)
- CSHL: Biological Data Science (Nov 9-12) -- Deadline Aug 26
- EMBL: From functional genomics to systems biology (Nov 15-18)
	- https://www.embl.org/about/info/course-and-conference-office/events/omx22-01/
- MLCB (Nov ?) -- Deadline Sep
- NeurIPS (Nov 26 - Dec 4) -- Deadline May
- EMBL: The complex life of RNA (Oct 12-15)
	- https://www.embl.org/about/info/course-and-conference-office/events/ees22-10/


_____________________________________________________________
## Other Resources

* _Markdown_ ([Link](https://guides.github.com/features/mastering-markdown/), 
     [Link](https://help.github.com/en/articles/basic-writing-and-formatting-syntax), 
	[Link](https://help.github.com/en/articles/working-with-advanced-formatting))
* _Github_ ([Link](https://education.github.com/git-cheat-sheet-education.pdf), 
	[Link](http://try.github.io/), 
	[Link](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf))



________________________________________________________________________________________
## Short Courses

	- DL/RL summer school (Due 4/1)
		- https://cifar.ca/next-generation/training-programs/deep-learning-reinforcement-learning-summer-school/
	- Oxford ML summer school (Applications open 2/14-4/15 -- Due 8/7-8/10))
		- https://www.oxfordml.school/
	- Princeton's Deep learning theory (Due 3/31)
		- https://deep-learning-summer-school.princeton.edu/#Apply
	- Machine learning summer school (Due ?)
		- http://mlss.cc/index.html

#### ML/DL
* _Deep Learning Summer School (Jul - Deadline March)_
([Website](https://dlrlsummerschool.ca/))
* _Machine Learning Summer Schools (August - Deadline: April)_
([Website](http://mlss.cc/)) 
* _Deep Learning Theory Summer School at Princeton (July - Deadline: March)_
([Website](https://deep-learning-summer-school.princeton.edu/#Apply)) 
* _Deep Learning for Natural Language Processing (2 sessions: summer and winter)_
([Website](http://ixa2.si.ehu.eus/deep_learning_seminar/)) 
* _NYU AI School (Jan 4-8 - Deadline: ?)_
([Website](https://nyu-mll.github.io/nyu-ai-school-2021/)) 
* _Janelia ML workshop (March-April - Deadline: Nov):_
([Website](https://www.janelia.org/you-janelia/conferences/workshop-listings)) 


Watch previous courses:
* _Deep Learning Summer School (2019)_
([Video](http://videolectures.net/DLRLsummerschool2018_toronto/)) 
* _Machine Learning Summer School 2019 - London_
([Website](https://sites.google.com/view/mlss-2019/home?authuser=0), 
[Video](https://sites.google.com/view/mlss-2019/lectures-and-tutorials?authuser=0)) 


#### Articles/Blogs
* _10 tips for writing CS papers_ ([Link1](http://www.nowozin.net/sebastian/blog/ten-tips-for-writing-cs-papers-part-1.html), [Link2](http://www.nowozin.net/sebastian/blog/ten-tips-for-writing-cs-papers-part-2.html))
* _Statistical Significance_ ([Link](https://www.annualreviews.org/doi/abs/10.1146/annurev-statistics-031219-041051?journalCode=statistics))
