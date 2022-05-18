# Miniconda-Bioconda
Working with  Miniconda and Bioconda to install bioinformatic tools
## What are Anaconda, Miniconda and Bioconda?
Before starting, I suggest you take a look at this great [source](https://www.biostars.org/p/9480933/) that explains in detail the terms we will be using along the tutorial. Briefly, Anaconda contains hundreds of packages among which is conda. Conda is a “package manager”, that is, a program that installs packages and all the dependencies that they need to work. Miniconda is a “mini” version of Anaconda that contains less packages, but DOES include conda. 

Some people argue that Anaconda takes too much space (~ 3GB) and you end up with many packages you don’t need. An alternative is to install Miniconda (which only includes conda, Python, and the packages they depend on) and then install new packages as you come to need them.
Finally, Bioconda is simply a channel (similar to a repository) from where you can download and install loads of packages related to bioinformatics.
In this tutorial, we will use Miniconda and Bioconda to install bioinformatics tools.
### Install Miniconda
First, run this command to go to the tmp folder in the root directory of your machine:
```
cd /tmp
```
Once there, run this command to download a Miniconda installer from the web:
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```
Once downloaded, you need to execute the script to start the installation of Miniconda. Use this command:
```
bash Miniconda3-latest-Linux-x86_64.sh
```
At some point of the installation, you have to accept the terms (just type yes) and then you have to confirm that you want to install Miniconda in the default location. I decided to accept the default location. The installation will continue and then you will be asked :
```
Do you want the installer to initialize Miniconda3 by running conda init? [yes|no]
```
At this stage, if you type [yes], you will have to close the terminal and open a new one for this option to take effect (you will get a warning about this). What will happen is that the Miniconda environment will activate by default anytime you open the terminal, so your command prompt will look something like this:
```
(base)jimena@DESKTOP-XXXXX:~$
```
If you change your mind and decide that you'd rather not have the conda base environment activate by default, you can use the following command:
```
(base)jimena@DESKTOP-XXXXX:~$ conda config --set auto_activate_base false
```
For this change to activate, you have to close the terminal and open a new one. Your command prompt should look like this:
```
jimena@DESKTOP-XXXXX:~$
```
To confirm that Miniconda was installed, type the below command and you should see a list of programmes/packages on your screen.
```
conda list
```
Done! In the next step, you will add the bioconda channel and start using it to install bioinformatic software :)
### Add Bioconda channel