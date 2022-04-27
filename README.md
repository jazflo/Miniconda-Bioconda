# Miniconda-Bioconda
Working with  Miniconda and Bioconda to install bioinformatic tools
## What are Anaconda, Miniconda and Bioconda?
Before starting, I suggest you take a look at this great [source](https://www.biostars.org/p/9480933/) that explains in detail the terms we will be using along the tutorial. Briefly, Anaconda contains hundreds of packages among which is conda. Conda is a “package manager”, that is, a program that installs packages and all the dependencies that they need to work. Miniconda is a “mini” version of Anaconda that contains less packages, but DOES include conda. 

Some people argue that Anaconda takes too much space (~ 3GB) and you end up with too many packages you don’t need. Therefore, an alternative is Miniconda (which only includes conda, Python, and the packages they depend on) and then install each package you need separately.
Finally, Bioconda is simply a channel (similar to a repository) from where you can download and install loads of packages related to bioinformatics.
In this tutorial, we will use Miniconda and Bioconda to install bioinformatics tools.
