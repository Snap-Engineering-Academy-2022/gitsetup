# Create A Git Repo + Create your first branch on a Shared Repo


## ➡️ Create Your Own Git Repo 
1. Sign up for a GitHub account (free student account for extra perks)
2. On Github.com, create a new repo
3. Then in the terminal,  navigate to the folder that contains your current files. Once there, initiate your git repo:

```bash
git init
```

4. To check your status of your repo at any point, use this:

```bash
git status
```

5. Now we want to add the HTML, CSS, JS files that you were just writing. To add one file you want to commit:

```bash
git add FILENAME
```

6. To add all the files you want to commit at once:

```bash
git add .
"(only adds the files in the current folder)"

OR

git add -A
"(no matter where you are in the repo)"
```

7. Now let's take a "screenshot" of your code by "committing" the code.

```bash
git commit -m "add a message explaining what you did here"
```

8. We're going to create a new branch called 'main'

```bash
git branch -M main
```

9. Now let's tell our git repo on our local computer which github repo to push up to!

```bash
git remote add origin LINK_TO_YOUR_GITHUB_REPO
```

10. Finally, let's push

```bash
git push -u origin main
```

11. Git config in the terminal

```bash
git config --global user.name "Your Name"
git config --global user.email your.email@example.com
```
    
    
    ✅ **Check your understanding:** 
    
    - Can you explain add vs commit vs push in your own words?
    - What’s the difference between local and remote?
    - What is the difference between a branch on a shared repo vs your own repo?



## ➡️ Create A Branch on a Shared Repo

1. Clone the existing class repo

[Snap-Engineering-Academy-2022/classwebsite](https://github.com/Snap-Engineering-Academy-2022/classwebsite)


```bash
git clone https://github.com/Snap-Engineering-Academy-2022/classwebsite
```

2. Then go inside the repo you just cloned. 
```bash
git clone https://github.com/Snap-Engineering-Academy-2022/classwebsite
```

3. Create your own branch within the `classwebsite` repo (you can name the branch whatever you want; to keep it consistent, use your first name): 

```bash
git branch

git branch YOURBRANCHNAME

git checkout YOURBRANCHNAME
```
 💡 `git checkout -b YOURBRANCHNAME` allows you to combine the previous commands into one command

3. Now, use `mkdir yourname` to create a new FOLDER inside this repo. 

4. Copy-paste your index.html, style.css, and script.js from yesterday's activity (the album website you already started) INTO this new folder. 

3. Then add and commit your files as you would normally!

4. Then push to the remote repo. 
    - `git push -u origin branch_name` creates the remote branch (vs. `checkout -b`)

5. If you did this correctly, you should see your branch on the classwebsite github!

<img width="758" alt="image" src="https://user-images.githubusercontent.com/26272095/173702852-f57d7afe-d39e-4680-b177-2033617a8b8d.png">


## 🧠 Extra Commands for Reference
- Some more nifty commands you might find handy

```bash
git commit --amend

"(use this to edit a commit!)"

git push -f

"(then use force push to the github)"
```

```bash
git diff

"(use this to see what has changed in your code!)"
```

```bash
git stash

"(use this to get rid of your current changes that are not committed,
 it'll return your code to the state of your previous commit)" 

git stash pop 

"(use this to get the changes that you stashed away earlier)"
```

