# CSC396-HW2
# Working with Jupyter Notebooks in Git

This guide will help you set up your environment and learn how to commit and push Jupyter notebooks using Git and GitHub.

## Setup your environment

You will need to set up an appropriate coding environment on your computer. Minimally, you will need:

* [git](https://git-scm.com/downloads/)
* [Python (3.8 or higher)](https://www.python.org/)
* [Jupyter Notebook](https://jupyter.org/install)

## Check out a new branch

Before you start working on your Jupyter notebooks, create a new branch in your GitHub repository:

1. Go to the repository created for you by GitHub Classroom. It should look like `https://github.com/YourClass/assignment-<your-username>`.
2. Create a [branch](https://help.github.com/articles/creating-and-deleting-branches-within-your-repository/) through the GitHub interface.
3. Name your branch as `lastname_firstname_dev` (this naming convention is important).
4. Clone the repository and checkout your new branch:
   ```
   git clone -b lastname_firstname_dev https://github.com/YourClass/assignment-<your-username>.git
   ```

## Working with Jupyter Notebooks

1. Navigate to your cloned repository folder.
2. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```
3. Create or open the assigned Jupyter notebook(s).
4. Complete your work in the notebook(s), making sure to save your changes frequently.

## Committing and Pushing Jupyter Notebooks

Jupyter notebooks are JSON files with a `.ipynb` extension. Here's how to commit and push them:

1. Save your notebook in Jupyter.
2. Open a terminal/command prompt and navigate to your repository folder.
3. Stage your changes:
   ```
   git add YourNotebook.ipynb
   ```
4. Commit your changes:
   ```
   git commit -m "Descriptive message about your changes"
   ```
5. Push your changes to GitHub:
   ```
   git push origin lastname_firstname_dev
   ```

## Important Notes

- Jupyter notebooks contain output cells that can make diffs hard to read. Consider using [nbdime](https://nbdime.readthedocs.io/) for better notebook diffing and merging.
- Don't forget to save your notebook before committing!

## Submitting your work

To submit your assignment:

1. [Create a pull request on GitHub](https://help.github.com/articles/creating-a-pull-request/#creating-the-pull-request) from your `lastname_firstname_dev` branch to the `master` branch.
2. Ensure all your changes are included in the "Files changed" tab.
3. Do not merge the pull request.

Your instructor will review and grade your work from this pull request. Make sure to submit before the assignment deadline! Any commits made after the deadline will not be considered for grading.

## Grading

Your assignment will be graded based on correctly implementing the solutions to each problem described in the handout.

