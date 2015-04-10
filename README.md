# peace-corps-android
The Android Peace Corps volunteer openings app 

# Using their API
The API for getting job listings is open soruce and [available here with instructions](https://github.com/PeaceCorps/Volunteer-Openings-API).  (Hey look, they also use github!)

You can do a simple test to try out the API by running this in a terminal or command line interface that has the command curl:
```bash
curl http://www.peacecorps.gov/api/v1/openings/?keyword=teacher
```

You can also just directly paste queries into your browser to see results. Essentially, the app will parse the string of text returned. It is encoded in a JSON structure for which there are libraries to more convinient read and restructure.

# Getting started
If you are new to using git, go through the following short online tutorial. Using github for keeping up to date code is critical for wokring on team projects, *especially* with short timelines!

[https://try.github.io/levels/1/challenges/1](https://try.github.io/levels/1/challenges/1)

Quick start: Run these commands either in a terminal (mac) or use a git shell donwloadable from github, such as [for windows](https://windows.github.com/) or [for mac](https://mac.github.com/).

```bash
# downloads the current repository to your computer, and move into that directory
git clone https://github.com/TeamGlobalApps/peace-corps-android.git
cd peace-corps-android 
```

The above you run only the first time. It creates a folder on your computer with the source code, along with a hidden folder with some fancy stuff you don't need to worry about that makes git work. Make sure all code in the project is in this folder, ie never reference materials from outside the folder!

The following are commands you will use more frequently:

```bash
# after not working on the project for a little while, ALWAYS pull the most recent code from the master to your local copy
git pull

# (do some work, e.g. edit the README.md file)

# explicitly add files that you want to push back up and sync with the master after editing
git add README.md

# add implicitly all files that changed since you last pulled
git add -u

# check the status, green are files that will be part of the push, red are files that changed or are added that have not been added to the changelog
git status

# create a commit. This packages things together and allows you to add a required description for what you worked on
git commit -m "your comment here"

# now you actually push the code up to the main master branch on the server
git push origin master
```

If there are issues, it's possible you forgot to pull first and the server is complaining your local copy is out of date! Try git pull and then git push in that case.
