# Notebooks Website Template

This repository is a template for a notebook rendering website. To use it, simply click on the `Use this repository as a template` button and fill your version of it with your notebooks. Some observations:

- Only notebooks on the `notebooks` folder will be rendered. Currently, it only supports Python notebooks.
- All dependencies of all notebooks must be described on the `requirements.txt` file on the root of the repository.
- The website is a Github Pages that lives inside the `gh-pages` branch of the repository. Further observations about it will be on its README.
- You can add as many supporting folders and files as you want.
- Every Friday at 11:59 PM UTC and on every push to `main` a Github Action will run executing all notebooks inside the `notebooks` folder and will convert all of them into PDFs and HTML files. The HTMLs will be used for the website. Of course, you can change the files inside of the `.github` folder to change this behavior.
