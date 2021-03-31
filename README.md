[![Workflow to Convert Jupyter Noteboks](https://github.com/BlockScience/notebooks-website-template/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/BlockScience/notebooks-website-template/actions/workflows/main.yml)

# Notebooks Website Template

This repository is a template for a notebook rendering website. To use it, simply click on the `Use this template` button and fill your fork with your notebooks.  
After clicking the button, you **must** check the option **Include all branches**. Otherwise, the website will not be built.  
Some observations:

- Only notebooks on the `notebooks` folder will be rendered. Currently, it only supports Python notebooks.
- All dependencies of all notebooks must be described on the `requirements.txt` file on the root of the repository.
- The website is a Github Pages that lives inside the `gh-pages` branch of the repository. Further observations about it will be on its README.
- You can add as many supporting folders and files as you want.
- Every Friday at 11:59 PM UTC and on every push to `main` a Github Action will run executing all notebooks inside the `notebooks` folder and will convert all of them into PDFs and HTML files. The HTMLs will be used for the website. Of course, you can change the files inside of the `.github` folder to change this behavior.
- I have put some OS level dependencies on the `entrypoint.sh` script that are most common to build wheels for Python packages, but you can add more. Keep in mind that the container used is a Debian Buster one.
- You can erase this README.
