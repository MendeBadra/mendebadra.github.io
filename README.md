This is my main branch of my blog. I post here sporadically.


Following is the reminder to myself:


### Steady-State Workflow


Many of the initial configuration steps are one-time actions. Once you've setup your blog as described, the typical workflow will be the following:

1. Create a new folder in the *posts* directory, using lowercase letters/numbers with words separated by dashes. 
2. Create a Jupyter notebook in this directory with the same name and .ipynb extension.
3. Change the first cell of the notebook to raw, and add title information as shown below. Be sure the first and last lines are three dashes, `---`:

        ---
        title: Solving the Normal Equations
        date: 2024-02-09
        description: An investigation into solving the normal equations with Python
        categories: [Python]
        ---


4. Create your blog post (narrative text, code, plots, equations, etc.). Save your changes. 

5. From the Git client, navigate to the blog directory, then add and commit your changes:

        $ cd /path/to/blog
        $ git add --all
        $ git commit -m "Added second blog post."


6. Ensure master branch is checkout (it should already be), then run the following two commands:

        $ git checkout master
        $ quarto publish gh-pages

7. View your published content at [username].github.io. If my username is jtrive, my content will be available at *jtrive.github.io*.
