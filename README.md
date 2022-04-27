# Miniconda-Bioconda
Working with  Miniconda and Bioconda to install bioinformatic tools
## What are Anaconda, Miniconda and Bioconda?
Before starting, I suggest you take a look at this great [source](https://www.biostars.org/p/9480933/) that explains in detail the terms we will be using along the tutorial. Briefly, Anaconda contains hundreds of packages among which is conda. Conda is a “package manager”, that is, a program that installs packages and all the dependencies that they need to work. Miniconda is a “mini” version of Anaconda that contains less packages, but DOES include conda. 

Some people argue that Anaconda takes too much space (~ 3GB) and you end up with many packages you don’t need. An alternative is to install Miniconda (which only includes conda, Python, and the packages they depend on) and then install each package you need separately.
Finally, Bioconda is simply a channel (similar to a repository) from where you can download and install loads of packages related to bioinformatics.
In this tutorial, we will use Miniconda and Bioconda to install bioinformatics tools.
### Install MIniconda
Run this command to go to the tmp folder in the root directory of your machine:
```
cd /tmp
```
Once there, run this command to download a Miniconda installer from the web:
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```
