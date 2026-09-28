![Init](Images/MLTitle.jpg)
***
# Introduction

Welcome to the Python training and ML rotation for TECS CDT. In this repository you will find all the appropriate files and exrcises to complete the initial Python training and rotation.

## Conda Environment

To keep your work space clean and ensure all the necessary modules are installed it is recommended to use a new conda environment for the TECS training period. However the modules installed should set you up for future coding and machine learning in your research. This section will start by creating the `ml-chem-env` environment from a `.yml` file. *Note that the following instructions are currently designed for Windows users*. 

1. From this repository download the `requirements.yml` file into your TECSPython directory (this is in `\Environments`)
2. In your anaconda prompt (or GitBash) check there is the `requirements.yml` file
3. Read the `requirements.yml` with Notepad++ and see what programs you will be installing
4. You will now need to type the command `conda env create --file requirements.yml`
5. Now to use the modules (programs) in this environment type `conda activate chem-ml-env`

By following these steps you should be able to use all the Jupyter Notebooks in the training period.

## GitHub Repository

You can also create your own GitHub repository to keep control of files and have version control. You can either make a new repository from scratch or you can clone an exisiting repository. Here the current repo will be cloned. In order to achieve this follow these instructions:

1. On the code tab copy the URL for the repo
2. In your anaconda prompt (or GitBash), in an appropriate location use the following command: `git clone [your-repository-url]` (where this is the URL you copied).
3. You should now see that a new directory has been made for this repo, check that all the files are there
4. By cloning this repo it is synced with this GitHub repo, you want to make your own repo, so the first step is to remove the link, on your anaconda prompt (or GitBash) cd into the repo
5. Running the command `git status` should indicate that this is synced
6. Remove the .git file with `rmdir /s /q .git` if you are using an anaconda prompt or `rm -rf .git` if you are using GitBash
7. Running `git status` will now show that you have removed the .git files and the directory is no longer linked to this GitHub repo
8. Run `git init` to initialize new .git files
9. Using `git add .` will take all the files in this directory and get them ready for staging (you can again see this with `git status`
10. Commit the files staged with `git commit -m "Initial commit"`
11. On the GitHub website make a new repository, you can name this what you want, with any description. Set the repo to private and do not initiate with a README, .gitignore and license, as these are already copied from your directory
12. There should now be some helpful instructions, you want to push an exisiting repo from the command line, therefore run `git remote add origin [your-repository-url]`
13. Set the branch with `git branch -M main`
14. Then finish with `git push -u origin main`, if you now refresh the GitHub webpage, you will now see that it reflects the files stored on your computer

Overall, you have cloned a GitHub repo adding it to your computer, you have then unsynced it, and set it up as a new repo hosted on GitHub. 

## GitHub Push

In the GitHub repo you have access to all the Jupyter Notebooks, once you have completed a Jupyter Notebook you will want to sync the changes on the GitHub website. In the folder where the repo has been set follow these instructions:

1. The command `git status` will show which files have been changed
2. Now stage the changes with `git add .`
3. These changes need to be committed, given you have completed the first notebook this could be `git commit -m "Notebook 1 complete"` the words in the speach marks can be any description
4. To sync with the GitHub repo use `git push`, now if you check online you should have a new commit which shows version history, and the changes should have been made.

## GitHub Working Together

GitHub has the option to add collaborators to GitHub repo, this allows people to work together in real time. Although details will not be specified here, you can make new branches and pull request allowing a dynamic way to work.

## Machine Learning Training

This repo will be updated with the files required for the ML training, in the directory `ML_Rotation` 1 to 6.
