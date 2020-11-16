# Week 7 (11/16): Midterm Presentations Part II
| Presenter(s) | Topic |
|---|---|
|Karen & Natalie	|  |
|Wendy & Sasha	|  |
|Donna & Daniel	|  |
|Anny	|  |
|Robyn	|  |
|Cynthia & Gerrlyn 	|  |
|Rayne	|  |
|Sami & Isabel	|  |
|Alejandro & Mike	|  |

Note that Dani and Andres will be presenting next week.

## Conversation Series for Week 8: Adam Millard-Ball
![Adam](https://cdn.theconversation.com/avatars/1123988/width238/file-20200709-46-1wmq6nl.jpg)

Make sure to read one (or more) of the following papers by Adam:
- The PNAS street-network sprawl paper (https://www.pnas.org/content/117/4/1941) is the most elaborate and gets into OSM and street connectivity metrics
- The parking paper (https://authors.elsevier.com/a/1bvYg,M0mRH3NY) is a nice example of dealing with GPS data
- The street width paper ([link-requires password](https://ucla.box.com/s/t6rah5b7pvkjp9vrqxzyafi7n15unswr)) is still a draft, and is simpler in terms of the data science angles but might be more accessible.

## Lightning Lecture
* The anatomy of a function

# Individual Assignment
Choose and read one of the journal papers authored by Adam (listed above). Write a one paragraph reaction to the article, and come up with two questions for the author.

Submit the assignment in your github class repository. There is no need to email the instructor, as long as the submission is up on your repo, and has a datestamp prior to midnight on Sunday.

# Group Assignment #3: A "functional" notebook

There are two components to this group assignment.

## A "clean" notebook

The midterm was an exploration of the many datasets and methods for your final project. It documented experimentations, failures, and successes along the way. It also exposed the challenges of working on a team, with potentially multiple notebooks to deliver different outputs. For this group assignment, take the time to eliminate the unnecessary content, and boil it down to the bare minimum necessary components that will dictate your final project. Your clean notebook should only include data that will be used in your project, followed by charts and maps that inform your research inquiry. Begin to tease out the narrative that will give life to your data. Each data wrangling step and data visualization should be followed by a markdown cell that succinctly explains what you are visualizing and how it is relevant. What story does it tell? How do the visuals enrich, confirm, or contradict the descriptive statistics you calculated earlier? Begin to explain the "why" and not just the "how" of your narrative: Why does this data address your research question? You are welcome to submit multiple notebooks, as long as they are sequenced in a clear and logical manner. Feel free to add any additional material that advances your project.

## Add a function

In addition to the task of cleaning up the notebook(s), include one or more functions in your data workflow. Functions can dramatically cut down the amount of code needed in your project. For example, consider a situation where you may want to produce multiple maps that display crime for different neighborhoods. You could create multiple cells with the code to create these maps... or, you can create a function that takes in an argument for `neighborhood` that then generates the map:

```python
# function
def crime_by_neighborhood(place):
    # code to create the crime map

# call the function
crime_by_neighborhood(place='Downtown')

````

At the end of the notebook, include a markdown cell that identifies each group member and describes their contribution to this assignment (one sentence each).

Make sure your notebook runs from the top without any errors and that all the visuals can be seen inline (without me having to re-run your notebook). 
