#error: failed to push some refs ...

This means your remote branch is different from your local branch 


```error: failed to push some refs to 'https://github.com/joeappleton18/cda401.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.```

**fix**

Simply pull from your remote branch. For example if you're working on master. 

```git pull origin master```

