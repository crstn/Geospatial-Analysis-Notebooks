# Geospatial Analysis Notebooks

Jupyter Notebooks for the PhD Course on [Python for Geospatial Analysis](https://phdcourses.dk/Course/73296) at Aalborg University Copenhagen, Spring 2020.

Please [fork](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) this repo so you have your own copy to work on during the course. We may also post some updates during the course, so forking is a better option than simply downloading it. 

The materials provided here assume basic knowledge of Python, so please make sure that you have gone through the following preparation steps before starting with the course:

1. Install the [Anaconda Distribution](https://www.anaconda.com/distribution/) for Python on your computer and work through the [Getting started with conda](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html) tutorial.
1. Read [A Whirlwind Tour of Python](https://www.oreilly.com/programming/free/files/a-whirlwind-tour-of-python.pdf) up to the end. The examples are also a good opportunity to take your shiny new Python installation for a test-drive, so feel free to play around with them. Alternatively, you can go through the Jupyter [notebooks](https://github.com/jakevdp/WhirlwindTourOfPython) associated with the book available on GitHub.

1. We'll be using [GitHub](https://github.com/) for some parts of this course. If you are new to Git,
	- Read the [Git Handbook](https://guides.github.com/introduction/git-handbook/).
	- Create an account on [github.com](https://github.com/) if you do not have one yet.
	- Install [GitHub Desktop](https://desktop.github.com/) on your computer ([tutorial](https://help.github.com/en/desktop/getting-started-with-github-desktop)).

Optional, but recommended:

1. Read [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) if you are new to Markdown.
1. Sign up for the [GitHub Student Developer Pack](https://education.github.com/pack) to get free access to some of the paid features on GitHub and some other tools/platforms.

## Setting up the course environment

The file [geoanalysis.yml](https://github.com/crstn/Geospatial-Analysis-Notebooks/blob/master/geoanalysis.yml) contains a specification of a virtual environment with all the Python modules needed for this course. To get up and running:

1. Create a new environment from the file, either by running `conda env create -f geoanalysis.yml` on the command line, or by [importing it in Anaconda Navigator](https://docs.anaconda.com/anaconda/navigator/tutorials/manage-environments/#importing-an-environment). This is going to take a while, we are now downloading a bunch of modules and all of their dependencies.
2. Activate the environment by typing `conda activate geoanalysis`, then `jupyter notebook`. Alternatively, in [Anaconda Navigator](https://docs.anaconda.com/anaconda/navigator/tutorials/manage-environments/#using-an-environment), click the arrow button next to geoanalysis, then choose Jupyter Notebook.