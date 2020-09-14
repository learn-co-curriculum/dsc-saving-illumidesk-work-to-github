# Saving Your Work from Illumidesk to Your GitHub Profile  

## Introduction  

In this lesson you will learn how to save the work you are doing to your personal GitHub profile.  This process should be done once the lesson has been completed.  This will be done through creating a fork of the lesson, changing the origin that git pushes to, and pushing the changes using a terminal in Illumidesk. After following this process, your contributions graph will register your work.

> "Earning green squares on your contribution graph means celebrating the work you do in open source and public projects. Starting today, you can also celebrate the work you do in private by sharing anonymized contributions from private repositories."- Sarah Vessels, The GitHub Blog

Learn more about how contributions are counted [Here](https://docs.github.com/en/github/setting-up-and-managing-your-github-profile/viewing-contributions-on-your-profile).  

## Objectives  

You will be able to:  

- Change the origin your information is pushed to in GitHub  
- Save your work from Illumidesk to GitHub
- Open a new terminal in Illumidesk  
- Earn credit for your work on your GitHub contribution graph  
<!--
## ! Bang  

Before we bigin this process, a quick note about a character we will be using.  Some of the commands we will be using are normally executed in Terminal or Command Prompt, but we will be sending our commands to the terminal from Jupyter Notebook with the (`!`) Bang.  Prepending a command with the (`!`) will allow you to execute terminal commands from the notebook.

Learn more about (`!`) Bang [Here](https://anaconda.zendesk.com/hc/en-us/articles/360023858254-Executing-Terminal-Commands-in-Jupyter-Notebooks#:~:text=In%20Jupyter%20Notebook%20you%20can,you%20are%20trying%20to%20use.)
-->
## Fork the Repo from GitHub  

- Navigate to the lesson's repsitory from Canvas using the GitHub repository link  

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/octacat.png' width='200'>  


- Click on the `Fork` link in that repository  

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/fork-repo.png' width='600'>  


- This will create a forked copy in your GitHub profile 

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/forking.png' width='300'>  


- You will be taken to your new repository once the forking is complete  

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/your-fork.png' width='600'>  


- Copy the url for this repo to your clipboard for use after a few more steps

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/your-fork-url.png' width='600'>  


## Open the lesson in Illumidesk  

The next step of the process can mostly be done in a Jupyter Notebook, but it is a good opportunity to get familiar with command line operations or working in Terminal, so we will do this part in a terminal in Illumidesk

- Open your Illumidesk control panel by clicking on the `Control Panel` button in the upper right corner of the notebook.

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/control-panel.png' width='600'>  


- Click on the `My Server` button to access your Illumidesk files  

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/my-server.png' width='600'>  


- Click the `New` drop down menu and choose `Terminal` and locate the command prompt   

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/new-terminal.png' width='600'>  


- Navigate to the directory of the lesson using the `cd` command followed by the name of the repository which begins with `dsc-`:  
```
cd <your lesson directory here>
```

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/cd-repo-name.png' width='600'>  


## Change the Origin URL for GitHub  

- Change the remote location that GitHub will push your work to using `!git remote set-url origin` and the repo location you copied to your clipboard from the fork you created in the first steps of this lesson.  

```
git remote set-url origin <your copied fork url here>
```

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/set-origin.png' width='600'>  



#### Stage and Commit Your Work

- Now that you have set the origin to your forked repository, you can stage and commit your work.  

```
git add .
```  

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/stage-changes.png' width='600'>

```
git commit -m '<your message here>'
```

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/commit-changes.png' width='600'>  



#### Push Your Work to GitHub  

- Now that you have staged and commited your work, you are ready to complete the task by pushing the changes to GitHub. The `push` command will prompt you to enter your GitHub username and password before your push can be completed.  

```
git push
```  

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/push.png' width='600'>  


- Enter your GitHub user name  

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/user-name.png' width='600'>  


- Enter your password  

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/password.png' width='600'>  


- If everything goes as planned, it should look something like this:  

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-saving-illumidesk-work-to-github/master/images/success.png' width='600'>


## Summary  

In this lesson, you were able to save the work you have done to your personal GitHub profile so you can begin showing activity on your GitHub profile.  Below is a block containing all of the code used in this process:

```
cd <your directory here>
git remote set-url origin <your repository url here>
git add .
git commit -m '<your message here>'
git push
```