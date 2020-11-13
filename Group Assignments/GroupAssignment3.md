# Group Assignment #3: Spatial Summaries

There are two components to this group assignments.

## A "clean" notebook

The midterm was an exploration of the many datasets and methods for your final project. It documented experimentations, failures, and successes along the way. It also exposed the challenges of working on a team, with potentially multiple notebooks to deliver different outputs. For this group assignment, take the time to eliminate the unnecessary content, and boil it down to the bare minimum necessary components that will dictate your final project. Your clean notebook should only include data that will be used in your project, followed by charts and maps that inform your research inquiry. Each visualization should be followed by a markdown cell that succinctly explains what you are visualizing and why it is interesting. What story does it tell? How do the visuals enrich, confirm, or contradict the descriptive statistics you calculated earlier? For the "bad" visualization and its improvement, explain what's wrong with the former and how you improved it with the latter. You are welcome to submit multiple notebooks, as long as they are sequenced in a clear and logical manner.

## Add a function

In addition to the task of cleaning up the notebook(s), include one or more functions in your data workflow. Functions can dramatically cut down the amount of code needed in your project. For example, consider a situation where you may want to produce a map that summarizes crime for different neighborhoods. You can create a function that takes in an argument for `neighborhood`:

```python
def crime_by_neighborhood(neighborhood):
    
````



At the end of the notebook, include a markdown cell that identifies each group member and describes their contribution to this assignment (one sentence each).

Make sure your notebook runs from the top without any errors and that all the visuals can be seen inline (without me having to re-run your notebook). 
