#Assignment Tips  (Due 15th May 2017)


##Ensure you have a gitHub repository set up

You'll need to set up a gitHub repository which will contain your work. [You can do this by clicking the following link](https://classroom.github.com/assignment-invitations/ef1d911f912b1ee82184bfbbca959320).


##Initial setup 

- Add a few initial files to your project 

- Initiate a git repository in your project folder `git init`

- Make your initial commit

```
git add -A
git commit -m "initial commit"
```

- Push your work up to gitHub 

```
git remote add origin 'your git repository address'
git push -u origin master
```


###Follow the GIT workflow introduced in class

-  Create new features on a feature branch `git checkout -b 'feature_branch'`. The name of the feature branch should be descriptive of the feature. 

- Commit regularly   `git commit -m 'commit message'` the commit should be descriptive of the work you have done. e.g "added menu links". **The commits should tell a story**

- If you make a mistake you can remove reset your work back to the last commit. `git reset --hard`

- At then end of the session push your master branch to gitHub

`git push origin master`

- If you've finished with your feature branch you can delete it

`git branch -d feature_branch`

- If you've not finished with your feature branch and want to push it to gitHub

`git push --set-upstream origin 'feature_branch'`

####Hint, you can work on your projects on multiple computers 

- First and only once per computer, you need to clone the repository:

`git clone repository_adress`

- Make sure you run `git pull origin` this ensures that you have the latest changes 


###Make sure you follow practice


All pages:  
* Git and GitHub should be used to version control your work
* Should have an intuitive menus and navigation that appear similar in look and feel 
* Should use external CSS
* Should contain valid HTML
* Should be clear sections using either `<div>`s or more semantically descriptive **html5** elements e.g.`<article> <aside> <footer> <header> <main> ...`  
* Should make Good use of `<title>` and `<meta>` tags, complying to SEO best practice 
* Should have intuitive comments within the html
* Should correct use of indentations to lay out the code 
* Should have a favicon 
