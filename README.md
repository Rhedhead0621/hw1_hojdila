# HW1_Hojdila

Information on using this cookiecutter

Development workflows
=======================

Create new project
----------------------

You've already done this if you are reading this file. You ran:

```bash
cookiecutter gh:Rhedhead0621/cookiecutter-datascience-simple
```

Put project under version control
---------------------------------

Let's get version control set up. You don't absolutely have to do this, but you should. For the local repository, do;

```bash
git init
git add .
git commit -m "Initial commit"
```

For the remote repository, make a github repository named HW1_Hojdila, then do;

```bash
git remote add origin git@github.com:Rhedhead0621/HW1_Hojdila.git
git branch -M main
git push -u origin main
```

Great. Using version control is good.


Folder structure
-----------------

Here's the folder structure that gets created by `cookiecutter-datascience-simple`:

	├── HW1_Hojdila	<- Your notebooks and scripts will live in the main project folder
		│   .gitignore					<- Common file types for git to ignore
		│   README.md					<- The top-level README for developers (you) using this project
		│   template-nb.ipynb			<- A Jupyter notebook template
		│
		├───data						<- Final and intermediate data
		│   └───raw						<- The original, immutable data dump
		│
		├───docs
		│       notes.md				<- Simple markdown template for project notes
		│
		└───output
				readme.md				<- Guidance for using this folder


Documentation
--------------

In this very simple project structure template, we've just included a markdown file with some typical
section headings to use for project notes. Expand as desired. Later in the semester we will learn how to
use Sphinx with restructuredText to write and generate documentation.


Dataset Notes
--------------

https://www.kaggle.com/code/tomasmantero/predicting-house-prices-keras-ann

Feature Columns

id: Unique ID for each home sold
date: Date of the home sale
price: Price of each home sold
bedrooms: Number of bedrooms
bathrooms: Number of bathrooms, where .5 accounts for a room with a toilet but no shower
sqft_living: Square footage of the apartments interior living space
sqft_lot: Square footage of the land space
floors: Number of floors
waterfront: - A dummy variable for whether the apartment was overlooking the waterfront or not
view: An index from 0 to 4 of how good the view of the property was
condition: - An index from 1 to 5 on the condition of the apartment,
grade: An index from 1 to 13, where 1-3 falls short of building construction and design, 7 has an average level of construction and design, and 11-13 have a high quality level of construction and design.
sqft_above: The square footage of the interior housing space that is above ground level
sqft_basement: The square footage of the interior housing space that is below ground level
yr_built: The year the house was initially built
yr_renovated: The year of the house’s last renovation
zipcode: What zipcode area the house is in
lat: Lattitude
long: Longitude
sqft_living15: The square footage of interior housing living space for the nearest 15 neighbors
sqft_lot15: The square footage of the land lots of the nearest 15 neighbors

