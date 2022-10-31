# Induction test

***NOTE. Check this file regularly for updates***

versions
* 2022-10-31. First draft


We invited applications (now closed) for the 2022-10 intake. As in [previous years]()  we have set an `induction task` to explore candidates' experience and skills. 
These tasks are based on our current projects, which are always dynamically changing. This year's reflects our Hackathons in Geneva, New Delhi, and OAWeek.


## purpose of internships

The purpose of these internships, in conjunction with the project manager, is to develop the use of semantic tools for 
enhancing and re-using climate knowledge. We have pioneered several approaches and you are asked to explore their use in this induction task:
* read UN IPCC climate change chapters using JupyterNotebooks
* create semantic dictionaries from the content. Clean and update the content using Wikidata references
* use the dictionaries to annotate chapter/s 
* use pygetpapers to automatically search the recent EuropePMC literature for climate-rich articles


The interns who join us will initially productise this approach and apply it to all the IPCC content (50+ chapters). 
We aim at automated approaches but there is always an element of error and cleaning. The result will be a semantic 
version of the IPCC reports (10,000 pages) and many dictionaries based on the content.  You will create resources to display the tools and their use

After this phase we hope to be joined by other groups. Possible examples
* creation of an IPCC/AR6 knowledge graph which can be queried with modern tools
* adaptation of #semanticClimate technology to other public reports such as IPBES.
* use of the dictionaries on current content such as preprints and theses.

We are looking for interns who are capable of working on modern informatics, in a flexible environment, in teams, 
learning new skills and working with a wide variety of other groups.

## details of tasks

Please watch this video before going to details of the tasks 
[click here](https://openvirus.slack.com/files/U02RK4A2FV1/F048V8US8Q4/abbreviation_keyword_extraction_video.mp4). It will help you to understand the jupyter Notebook.

Please complete each of the steps and document your results.

We would like to have your results/documentation by November [insert date]

### 1. content

Our initial content will be Chapter08 of IPCC WG3 Climate Change 2022: Mitigation of Climate Change](https://www.ipcc.ch/report/ar6/wg3/). Download chapter08
It's over 100 pages. We are developing tools to make it easier to read. Please read (**only**) the **first TWO paragraphs** of the Executive summary.

### 2. using Jupyter Notebooks (in Google Colab) to analyze the chapters

You should Analyze Chapter08 using [Jupyter Notebooks in Google Colab](https://colab.research.google.com/github/petermr/semanticClimate/blob/main/outreach/cambridge_presentation/Hackathon_Notebook/climate_hackathon_chapter08.ipynb). We expect this will be new for many of you; we want to see how well you can tackle new challenges. You can get help from the web or friends. We have already provided an HTML version of the chapter in the notebook. we will appreciate your efforts.

Q. Explain (1 sentence) the two types of `cell` in a Notebook.

The subtasks are:

### 3. Create abbreviation dictionary from the content
Q. What tool was used to create the dictionary?(Hint-https://github.com/petermr/docanalysis#readme)
Q. Where is the output dictionary?
Q. Explain the first `entry` in the dictionary.(download the dictionary from files in notebook)

### 4. Clean and update the dictionary using Wikidata references                                                                                             

* Q. find an entry with a single WikidataID (i.e. unambigous). Do you believe it is correct?
* Q. find an entry with ambiguous WikidataID references (i.e. more than one hit). Which, if any is the correct one? Why did the ambiguity arise?
* Q. (How) could we write software to resolve ambiguities? (outline only)
* Q. Find an entry **without** a wikidata reference and manually suggest an appropriate QID.


### 5. Use the dictionaries to annotate chapter/s 

Run the annotation cell and explain what it does notebook last cell. 

### 6. pygetpapers


`pygetpapers` was written by our volunteer Ayush Garg and is available at https://pypi.org/project/pygetpapers/. 

***Initially Limit your hits to 10 hits***

* install and verify it works
* create a query on Climate change in India using 2022 articles 
* download both PDF and XML
* manually inspect the first 5 hits and comment on whether they are useful to explore the query

## Summary

Describe (MAX 250 words) what you did, why it's useful, and one way it could be improved or expanded.

