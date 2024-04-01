# cintel-04-local

## Publish Interactive Reactive App

#### Virtual environment

-Create a repo in GitHub, clone it to down and create a local project virtual environment in the .venv folder using:

python3 -m venv .venv

-Activate

source .venv/bin/activate

-Install all the packages needed for the project

python3 -m pip install --upgrade pip setuptools
python3 -m pip install --upgrade -r requirements.txt

#### Run the App

shiny run --reload --launch-browser penguins/app.py

#### Build App

shiny static-assets remove
shinylive export penguins docs

#### Git Add / Commit / Push to GitHub

git add .
git commit -m "Your commit message"
git push -u origin main

#### Publish GitHub Pages for the Repo

1. Go to the repository on GitHub and navigate to the Settings tab.
2. Scroll down and click the Pages section down the left.
3. Select branch main as the source for the site.
4. Change from the root folder to the docs folder to publish from.
5. Click Save and wait for the site to build.
6. Eventually, be patient, your app will be published and if you scroll to the top of the Pages tab, you'll see your github.io URL for the hosted web app. Copy this to your clipboard. 
7. Back on the main repo page, find the About section of the repo (kind of upper right).
8. Edit the "About" section of the repository to include a link to your hosted web app by using the Pages URL. 