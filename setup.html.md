# Setup


<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->

## Step 0 - Install `nbdev`

Follow instructions from official page:
https://nbdev.fast.ai/tutorials/tutorial.html. This tutorial includes
the following installations:

- Install JupyterLab (using `pip` or `conda`)  
- Install `nbdev` (using `pip` or `conda`)  
- Install Quarto (using command from `nbdev`)  
- Install Quarto JupyterLab extension (command
  `pip install jupyterlab-quarto`)

**NOTE**  
It is possible that you encounter errors due to latest updates from
Jupyter Lab. One such error is JavaScript error when rendering notebook
caused when adding comments onto parameter declaration. One solution to
this is to downgrade Jupyter Lab version to 3, e.g.,

    conda install -c conda-forge jupyterlab=3

## Step 1 - Initialize repository

Follow the First steps Section of the same tutorial. The main steps are:

- Create and clone a new Github repository  
- Use command `nbdev_new` in the cloned repository to initialize a
  `nbdev` project  
- Follow the prompts to create a suitable `setting.ini` file

**NOTE**

- By default, the module automatically exported by `nbdev` will have the
  same name as the repository (if not set otherwise). The exported
  python files will be stored in a directory with the same name in root
  repository. Please be careful not to include inappropriate characters
  in the module name or source package, else the exported modules cannot
  be imported correctly.  
- By default, two Github actions are added after initialization - one
  for testing, and one for deploying automatically generated documents.
  However, for us it is better to remove the deploying actions (or
  writing new action just for generating documents). This is because
  deployiment is to `ninjalabo.github.io` by Github Pages, which is
  already occupied with our Landing Page.  
- By default, Apache LICENSE is added. But we can remove that file if
  repository is only for private use.

## Step 2 - Start making edits

Keep following the tutorial. From its Recap section:

- Install hooks for git-friendly notebooks with `nbdev_install_hooks`  
- Install your package for development with `pip install -e '.[dev]'`
  (automatic update)  
- Preview your docs with `nbdev_preview` (generate Quarto pages for
  documentation)  
- Add your changes  
- Update nbs/index.ipynb with your own information (this becomes the
  README.md file)  
- Prepare your changes with `nbdev_prepare`  
- Push to GitHub

For making changes, take a look at the example workflow in
`02_workflow.ipynb`.