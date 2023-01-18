# computational-physics-class-404-604-Spring-2023

Welcome to the course GitHub repository (repo) for __Computational__Physics__II__, at UNLV.  Here you'll find Jupyter Notebooks (`.ipynb`) that correspond to or suppplement in-class lectures.  If you're not familiar with [GitHub](#GitHub), [Jupyter](#Jupyter) or the [Python](#Python) programming language, please read through the relevant sections below.


## GitHub
1. First, create a GitHub account if you don't already have one at https://github.com/join.
2. Once you're logged in, "fork" our class repo by clicking the __Fork__ button in the header (usually upper-right) of [this page](https://github.com/zhuzh1983/computational-physics-class-404-604-Spring-2023).  Your fork is where you can make changes or upload ("commit") homework and other assignemnts.  For more information, see [Forking Projects](https://guides.github.com/activities/forking/).
3. If you're on a Mac or Windows machine, and are new to the _Git_ version-control system, we recommend using [GitHub Desktop](https://desktop.github.com/) to "clone" your forked repo to your local machine and upload homework assignments.  For more information on this application, see [Installing and configuring GitHub Desktop](https://docs.github.com/en/desktop/installing-and-configuring-github-desktop).  For more information on "cloning," see the [relevant subsection below](#Clo__[GitHub Desktop](https://desktop.github.com/)__ning).
4. To see how and why GitHub and Git are used to develop code and online OpenCourseWare, visit [Understanding the GitHub flow](https://guides.github.com/introduction/flow/).
5. For more information about GitHub, including how to ceate your own repository and commit changes, see the 10-minute [Hello World](https://guides.github.com/activities/hello-world/) guide.

### Cloning
When you "clone" using _Git_ (e.g., this repo, or your own fork), you create a local, asynchronous copy of a GitHub repo on your machine that you can modify: add, edit, or remove files.  These local modifications can then be "staged" as individual "commits," and later "pushed" (written) to the remote ("upstream") source from which the clone was made, provided you have the necessary write permissions (this is always the case for your own forks).

As recommended above, [GitHub Desktop](https://desktop.github.com/) provides an easy-to-use, graphical interface for the vast majority of common _Git_ commands and tasks, including cloning (e.g., `git clone`); see [Cloning and forking repositories from GitHub Desktop](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/cloning-and-forking-repositories-from-github-desktop) for more information.

Alternatively, if you have `git` installed, via the command line interface (CLI) or terminal, you can clone your fork of this repo to your current local directory (see [`pwd`](https://en.wikipedia.org/wiki/Pwd)) using,
```bash
$ git clone https://github.com/$USER/computational-physics-class-404-604-Spring-2022.git
```
where `$USER` is your GitHub username.

### Syncing your branch
Whenever new commits (e.g., additional lecture notebooks) are added to this class repo (i.e., the `upstream/master` relative to your fork), using GitHub Desktop you can __re-sync__ your fork as follows:
1. Below the top menu bar, click the __Fetch origin__ button; this will check for any recent changes made to this `upstream` repo.
2. From the top menu bar, click __Branch__>__Merge into current branch...__ (`Ctrl+Shift+M`)
3. Under the section __Other branches__, select "upstream/master" and click the button at the bottom "Merge __upstream/master__ into __master__".
4. For more information, or if you run into any issues (e.g., there are "merge conflicts"), see [Merging another branch into your project branch](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/syncing-your-branch#merging-another-branch-into-your-project-branch).


## Anaconda
We recommend using __Anaconda__ to manage your Python environments and to install JupyterLab.  Anaconda is one of the most widely used solutions for package management for Python and comes with 1,500+ popular packages out of the box, including the most common ones we will use in this course.  Below are instructions or external resources for setting up Anaconda depending on your operating system.

### Windows
The first step is to get Linux running inside your Windows machine using __WSL__.  Read and follow the _first three_ (3) sections of the [Get started with the Windows Subsystem for Linux](https://docs.microsoft.com/en-us/learn/modules/get-started-with-windows-subsystem-for-linux/) guide (i.e., "Introduction" through "Integration between Windows and Linux file systems").  We highly recommend installing __Ubuntu__ as your Linux distribution, for easibility and widespread support.

Once you have Linux installed and can access the terminal, you can install Anaconda with the following steps:
1. Open your Linux terminal (e.g., _Ubuntu_) and enter the following command to download _Miniconda_ (a lightweight version of Anaconda):
```bash
$ wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```
2. To install Miniconda, run: 
```bash
bash Miniconda3-latest-Linux-x86_64.sh
```
3. Follow the prompts on the installer screens.
4. If you are unsure about any setting, accept the defaults.  You can change them later.
5. To make the changes take effect, close and then re-open your terminal window.
6. Test your installation.  In your terminal window, run the command `conda list`.  A list of installed packages appears if it has been installed correctly.

### macOS
See [Installing Anaconda/Miniconda on macOS](https://docs.conda.io/projects/conda/en/latest/user-guide/install/macos.html).

### Linux
See [Installing Anaconda/Miniconda on Linux](https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html).


## Jupyter
If you do not already have Jupyter Notebook or Lab installed, we recommend setting up [Anaconda](#Anaconda) first (see above).  Below are resources and instructions for setting up Jupyter on your local machine, as well as usage guides and tutorials.  As __JupyterLab__ will eventually replace the classic _Jupyter Notebook_, we recommend setting up the former if this is your first time.

### Setup
1. Open your terminal.
2. Install JupyterLab with:
```bash
$ conda install -c conda-forge jupyterlab
```
3. [Start JupyterLab](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html).

### Tutorials
- [The JupyterLab Interface](https://jupyterlab.readthedocs.io/en/stable/user/interface.html)
- [Jupyter Lab Tutorial (YouTube)](https://www.youtube.com/watch?v=7wfPqAyYADY)


## Python
Once you have everything set up and working, please open in Jupyter `Lect1.ipynb` from your forked repo that is cloned to your local machine (see [Cloning and forking repositories from GitHub Desktop](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/cloning-and-forking-repositories-from-github-desktop) for more information or assistance).  Sections 1 and 2 of the notebook cover some basic interactive Python scripting in Jupyter, needed for assignemnts.

### Additional resources
- "Learn the Basics" section at https://www.learnpython.org/

## Assignments
You will be expected to upload your assignments (e.g., homework, group projects, etc.) by "pushing" your local commits to your fork.  Again, if you are using Windows of Mac, we recommend using [GitHub Desktop](https://desktop.github.com/) to visually simplify this process, while avoiding common issues and mistakes in the command line.  One added benefit of the graphical user interface (GUI) over the CLI of Git is the ability to preview an "inline diff" (line-by-line changes to a modified—i.e., existing—file) before making a commit.

For more information on these procedures, using GitHub Desktop, see the following guides:
- [Committing and reviewing changes to your project](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/committing-and-reviewing-changes-to-your-project)
- [Pushing changes to GitHub](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/pushing-changes-to-github)


## Questions or Issues
You can post any questions or issues you may have in a [Discussion](https://unlv.instructure.com/courses/76074/discussion_topics) on WebCampus (Canvas), where I or other students can respond with advice or troubleshooting tips.

If you find any technical issues with, or have suggestions (e.g., additional resources) for, this guide, feel free to open a new "issue" by clicking the __Issues__ tab near the top header of this repo (see [Mastering Issues](https://guides.github.com/features/issues/) for more information).
